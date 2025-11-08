Hetzner DynDNS (A-Records) based on a bash script.

Requirements: curl

You need an API Token: Your project > security > API-Tokens > Create one with read and write access.
You need your zoneID: run the zoneID script: "bash ./zoneID -t YOUR_API-TOKEN.

Now save your zoneID in the ddns.sh in ZONE_ID and also enter your API-Token in API-TOKEN.

With the flag -n you can enter your record name.

After that installing a cronjob with:

*/10 * * * *  bash ./ddns.sh -n Your-Record-Name 
