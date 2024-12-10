Title: Bulk Tweet Deletion Script

Description:
This script automates the process of bulk deleting tweets, retweets, and replies on X (formerly Twitter). It leverages the platform’s internal APIs to fetch timelines, filter tweets based on customizable criteria, and delete them at scale. Ideal for users who want to clean up their timeline, remove old or sensitive content, or maintain a curated presence without manually deleting each tweet.

Key Features:
	•	Archive-Based or Live Deletion:
	•	From Archive: Supports loading a tweets.js file from your official Twitter archive for quicker, more reliable bulk deletion.
	•	Live Deletion: If no archive is provided, it can iterate through your timeline to find and remove tweets directly.
	•	Fine-Grained Filters:
	•	Keyword Matching: Specify keywords or phrases. Only tweets containing these will be considered for deletion.
	•	Date Range: Delete tweets posted within a certain timeframe.
	•	Ignore List: Keep important tweets safe by whitelisting their IDs.
	•	Retweet Handling: Enable or disable the removal of retweets.
	•	Protected Deletions:
	•	Skip Pinned Tweets: Optionally ignore pinned tweets to avoid accidental removal of highlighted content.
	•	Stop Conditions: Automatically stop if no more tweets match your criteria, preventing unintended mass deletions.
	•	Robustness & Rate Limit Handling:
	•	Retries and delays are built in to handle network issues or rate limits gracefully.

Usage Overview:
	1.	Configuration:
	•	Update the authorization, client_tid, client_uuid, and username variables with your values.
	•	Set filters and behaviors in delete_options (e.g., from_archive, unretweet, keywords, date range).
	2.	Archive Mode:
	•	If from_archive is true, the script prompts you to upload your tweets.js file. Once confirmed, it parses the file and begins deletion automatically.
	3.	Live Mode:
	•	If from_archive is false, the script will fetch tweets directly from your timeline and apply your filters, deleting matches as it goes.
	4.	Monitoring & Logs:
	•	The script logs progress, showing which tweets it’s deleting, and any errors or retries it encounters.

Note:
Use responsibly. Deletions are permanent. Ensure you understand and trust the filters you’ve set before running the script. Make a backup of your tweets or test with a small sample before performing large-scale deletions.
