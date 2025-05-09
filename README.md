# memobase

**Repository:** [dify-plugin-memobase](https://github.com/ACAne0320/dify-plugin-memobase)

**Author:** acane0320

**Version:** 0.0.2

**Type:** tool

## Description

The Memobase plugin allows Dify applications to connect and interact with a user's **self-hosted or managed Memobase instance**. Memobase is an open-source long-term memory solution for AI. This plugin provides tools for managing users, conversation data, profiles, and events within that instance.

## Features

*   **User Management:** Add, get, update, and delete users in your Memobase instance.
*   **User Data Management:** Insert conversation data, retrieve specific or paginated data, delete data, and get personalized user context from your Memobase.
*   **User Profile Management:** Add, get, update, and delete user profile entries. Manage profile configuration and flush the memory buffer in your Memobase.
*   **User Event Management:** Get recent events, search events based on queries, update, and delete events within your Memobase.

## Setup

[Memobase](https://github.com/memodb-io/memobase) is open-source, allowing you to deploy your own instance.

To use this plugin, you need to provide the following credentials when adding it in Dify, corresponding to **your** Memobase instance:

1.  **Memobase URL:** The endpoint URL of **your** Memobase instance (e.g., `https://api.memobase.dev`).
2.  **Memobase API Key:** **Your** API key for authenticating with **your** Memobase instance.

You can obtain these from your [Memobase dashboard](https://www.memobase.io/en/dashboard) or configuration.
![Memobase dashboard](/_assets/memobase_dashboard.png)
### Usage

Once configured with the details of your Memobase instance, the Memobase tools will be available within the Dify orchestration interface.

You can add these tools to your workflows to:

*   Store conversation history for long-term memory in your Memobase.
*   Retrieve user profiles or context from your Memobase to personalize responses.
*   Search past user events or interactions stored in your Memobase.
*   Manage user information within your Memobase directly from Dify.

For specific instructions on how to use the tool, you can refer to the [Memobase API Reference](https://docs.memobase.io/api-reference/overview).

### Workflow
Here's a minimal workflow based on the memobase plugin to implement the memory functionality.
![Memobase workflow](/_assets/workflow.png)