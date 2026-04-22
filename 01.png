// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleDAO {

    struct Proposal {
        string description;
        uint voteCount;
        uint deadline;
        bool executed;
    }

    address public owner;
    Proposal[] public proposals;

    mapping(uint => mapping(address => bool)) public hasVoted;

    constructor() {
        owner = msg.sender;
    }

    // Create proposal
    function createProposal(string memory _description, uint _duration) public {
        proposals.push(Proposal({
            description: _description,
            voteCount: 0,
            deadline: block.timestamp + _duration,
            executed: false
        }));
    }

    // Vote on proposal
    function vote(uint _proposalId) public {
        Proposal storage proposal = proposals[_proposalId];

        require(block.timestamp < proposal.deadline, "Voting ended");
        require(!hasVoted[_proposalId][msg.sender], "Already voted");

        proposal.voteCount++;
        hasVoted[_proposalId][msg.sender] = true;
    }

    // Execute proposal
    function executeProposal(uint _proposalId) public {
        Proposal storage proposal = proposals[_proposalId];

        require(block.timestamp >= proposal.deadline, "Voting not finished");
        require(!proposal.executed, "Already executed");

        if (proposal.voteCount > 0) {
            proposal.executed = true;
        }
    }

    // View proposals
    function getProposals() public view returns (Proposal[] memory) {
        return proposals;
    }
}