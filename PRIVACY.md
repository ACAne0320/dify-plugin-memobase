## Privacy Policy for Memobase Plugin

This plugin acts as a client to interact with a user-provided Memobase instance. Memobase is an open-source project, allowing users to self-host their own instances.

**Data Collection:**

To function, this plugin requires the following credentials provided by the user during setup in Dify, corresponding to *their* Memobase instance (self-hosted or otherwise):
*   `memobase_url`: The URL of the user's Memobase instance.
*   `memobase_api_key`: The API key for authenticating with the user's Memobase instance.

When using the plugin's tools, the following data might be processed and sent to the specified Memobase instance:
*   `user_id`: Identifier for the end-user within Memobase.
*   User conversation data (user messages, assistant messages) for insertion.
*   User profile data (topic, sub-topic, content) for adding or updating profiles.
*   User event data (as JSON) for adding or updating events.
*   Search queries for events.
*   Metadata associated with users (as JSON).
*   Configuration data for Memobase profiles.

**Data Usage:**

*   The collected credentials (`memobase_url`, `memobase_api_key`) are used solely to establish a connection and authenticate with the user's designated Memobase instance.
*   Other data (like `user_id`, conversation content, profile details, event data, queries) is transmitted directly to the user's Memobase instance via its API to perform the requested actions (e.g., inserting data, retrieving profiles, searching events).
*   This plugin itself does not persistently store any user data or credentials beyond the necessary runtime context for executing the requested tool function. Data is passed through to the Memobase API.

**Third-Party Services / Self-Hosting:**

*   This plugin relies entirely on the user-provided Memobase instance. All data processed by the tools is sent to this instance.
*   Since [Memobase](https://github.com/memodb-io/memobase) is open-source , users typically deploy and manage their own instances.
*   Users are responsible for the privacy and security practices of their own Memobase instance. They should review the Memobase documentation and their specific deployment configuration to understand how data is handled.

**Contact:**

For questions regarding this plugin's privacy practices (specifically how it interacts with Memobase), please contact the author: [ACAne0320](https://github.com/ACAne0320). For questions about Memobase itself, please refer to the Memobase project resources.