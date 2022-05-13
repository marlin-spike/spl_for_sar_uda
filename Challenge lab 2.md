### Task 1: Create a bucket

1. Navigation menu > **Cloud Storage** > Browser > Create Bucket
2. Name your bucket > Enter **<Bucket Name>** > Continue
3. Use default for the remaining 
4. Create


### Task 2: Create a Pub/Sub topic

1. Navigation menu > **Pub/Sub** > Topics
2. Create Topic > **Name:** <Topic Name> > Create Topic


### Task 3: Create the thumbnail Cloud Function

1. Navigation menu > **Cloud Functions** > Create Function

2. Use the following config:

   **Name:** <Cloud Function Name>
   **Region:** us-east1
   **Trigger:** **Cloud Storage**
         **then add <Bucket Name>**
   **Event type:** Finalize/Create
   **Bucket:** BROWSE > Select the qwiklabs bucket

3. Remaining default > Next

4. **Runtime:** Node.js 14
   **Entry point:** thumbnail
5. Add the code appropiately

6. Download the image from URL

7. Navigation menu > **Cloud Storage** > Browser > Select your bucket > Upload files
8. Refresh bucket

### Task 4: Remove the previous cloud engineer

1. Navigation menu > **IAM & Admin** > IAM
2. Search for the "**Username 2**" > Edit > Delete Role

