const apiKey = "a706bdd8b99cb2433b12";
const apiSecret = "3ffd4d3ec27ea4e7a4b1cea7abcbe5dc5cc6056e2c9c898cb55304d75ac18175";

async function uploadFile() {
    const file = document.getElementById("fileInput").files[0];
    const resultDiv = document.getElementById("result");

    if (!file) {
        alert("Please select a file");
        return;
    }

    resultDiv.innerHTML = "⏳ Uploading...";

    const formData = new FormData();
    formData.append("file", file);

    try {
        const res = await fetch("https://api.pinata.cloud/pinning/pinFileToIPFS", {
            method: "POST",
            headers: {
                pinata_api_key: apiKey,
                pinata_secret_api_key: apiSecret
            },
            body: formData
        });

        const data = await res.json();
        const cid = data.IpfsHash;

        resultDiv.innerHTML = `
            Uploaded Successfully! <br><br>
            <b>CID:</b> ${cid} <br>
            <a href="https://gateway.pinata.cloud/ipfs/${cid}" target="_blank">
                🔗 View File
            </a>
        `;

    } catch (err) {
        console.error(err);
        resultDiv.innerHTML = "❌ Upload Failed";
    }
}

function getFile() {
    const cid = document.getElementById("cidInput").value;

    if (!cid) {
        alert("Enter CID");
        return;
    }

    const url = `https://ipfs.io/ipfs/${cid}`;

    // Try preview
    const iframe = document.getElementById("preview");
    iframe.src = url;

    // Also open in new tab (backup)
    window.open(url, "_blank");
}