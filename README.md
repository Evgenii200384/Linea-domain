# Linea-domain
import { Linea } from "@thirdweb-dev/chains";
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

// If used on the FRONTEND pass your 'clientId'
const sdk = new ThirdwebSDK(Linea, {
clientId: "YOUR_CLIENT_ID",
});
// --- OR ---
// If used on the BACKEND pass your 'secretKey'
const sdk = new ThirdwebSDK(Linea, {
secretKey: "YOUR_SECRET_KEY",
});

const contract = await sdk.getContract("0xeD5DC729AAa8d9BD4D09CD4cc0C51eBdA5d4286C");
