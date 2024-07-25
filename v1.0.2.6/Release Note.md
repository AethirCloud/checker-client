Release Date: July 17, 2024

Version: CheckerService, GUI V1.0.2.6, CLI V1.0.2.6

Mandatory Update: Yes

Updates:

To enhance system stability and security, we are implementing a series of important system upgrades.

1. Burner Wallet Registration Flow: 

A new burner wallet address will not be registered in the Checker System, until an owner delegates to that address. While there is no difference in your user experience, you now cannot establish websocket connection to the Checker System until you are registered.

So if you created a new burner wallet, you will now need to wait until a license owner initiates delegation flow, for your checker client to establish connection to the Checker System. The Checker System picks up such registration requests every 5 minutes. Please note, there is now a rate limit on the register endpoint, allowing one request per minute per IP. Exceeding this limit will result in the IP being blacklisted for the day

2. API Token:

API tokens will now have an expiration time and need to be present in all API requests. Tokens are automatically refreshed.

All API requests will now be subject to rate limits.

3. Wget Restrictions: 

Wget requests will also require a valid token.

Any IP with download volumes exceeding normal threshold will be restricted.

This upgrade is mandatory and scheduled to take place on July 17th. If you are using CLI, this upgrade will happen automatically in the background as long as your client and service are up; if you are using Windows, please make sure you confirm on the update popup. If you have any questions, please don’t hesitate to reach out in discord!
