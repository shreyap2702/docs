# Autosend Python SDK

This SDK provides a simple Python SDK for the AutoSend Email API.
It removes the need to manually build HTTP requests, manage payloads, or handle API endpoints.

If you want to send transactional emails, bulk messages, or manage contacts from Python, this SDK provides a clean and consistent way to do it.

 ## SDK and Client

 The Autosend Python SDK exposes a primary client class, `AutosendClient`, which wraps the AutoSend HTTP API and provides high-level helper methods for common tasks.

 Key responsibilities of the SDK / client:

 * Request formatting and payload construction
 * Validation and error handling
 * Sending transactional and bulk emails
 * Managing contacts (create/update/upsert, search, remove)

 Initialization is simple — you only need your API key. Example:

 ```python
 from autosend import AutosendClient

 client = AutosendClient(api_key="YOUR_AUTOSEND_API_KEY")
 ```

 Once initialized you can use methods such as `send_email`, `send_bulk`, and `upsert_contact` to perform common operations (see the Quickstart and API reference in this docs site for examples).

 The SDK aims to make integration fast and reliable by handling the low-level HTTP work so you can focus on your application logic.
