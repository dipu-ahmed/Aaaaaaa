import Appwrite

let client = Client()
    .setEndpoint("https://[HOSTNAME_OR_IP]/v1") // Your API Endpoint
    .setProject("5df5acd0d48c2") // Your project ID

let databases = Databases(client)

let result = try await databases.deleteDocument(
    databaseId: "[DATABASE_ID]",
    collectionId: "[COLLECTION_ID]",
    documentId: "[DOCUMENT_ID]"
)

