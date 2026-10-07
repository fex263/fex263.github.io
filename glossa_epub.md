---
layout: default
title: README
---
# OpenReader Privacy Policy

Effective date: [YYYY-MM-DD]　Version: 1.0
Developer: [Developer name]　Contact: [contact@example.com]

OpenReader ("the App") is a local Windows desktop app for reading EPUB books, with an optional feature that translates book text using a Large Language Model (LLM) service **that you configure yourself**. This policy explains what data the App handles, where it goes, and your choices.

## 1. Summary

- The App has **no developer-operated server**. We **do not collect, receive or store** any of your data.
- The App has **no accounts, no advertising, and no third-party analytics or telemetry**.
- Book text is sent to an external LLM service **only if you configure one and use the translation feature**, and only to the endpoint **you specify**.

## 2. Data the App handles

All of the following data is stored **locally on your device only**:

| Data | Purpose |
|---|---|
| Book files and metadata (title, author, chapters, file path) | Library display and reading. |
| Reading progress, bookmarks, reading settings, window position | Restoring your reading state. |
| Translation cache (translated chapter text) | Avoiding repeated translation. |
| Your LLM configuration: endpoint URL, model name, **API key** | Calling the LLM service you chose. |
| Diagnostic logs (runtime status, error messages) | Troubleshooting. They are not uploaded. |

The App does not access files other than those you choose to import, and does not collect device identifiers, location, or contacts.

## 3. Book content sent to third-party LLM services

1. When you use translation, the **book text** you chose to translate (plus translation instructions) is sent over the network to the LLM endpoint you entered in settings.
2. That service is **entirely your choice**. It may be a third-party cloud service (e.g. OpenAI, Anthropic, Google Gemini, DeepSeek, Alibaba Cloud, Zhipu, SiliconFlow) or a service on your own machine or network (e.g. Ollama, LM Studio).
3. Once data is sent, its processing, storage, retention, and any use for **model training** are governed by **that provider's privacy policy and terms**, not by us. **Some providers may log your inputs and may use them to train models.** Please review the provider's policy and, if needed, choose one that lets you opt out of training or that runs locally.
4. Even when you use a local service such as Ollama, the App still sends the content to the endpoint you specified; that endpoint just happens to be local.
5. The App does not, and cannot, send content to any other destination without your knowledge.
6. If no LLM service is configured, the App **makes no network requests involving book content**.

## 4. API keys

- Your API key is stored in a configuration file on your device. **It is currently stored in plain text (not encrypted).** Do not use the App on untrusted computers or shared accounts, and prefer keys with limited permissions that you can revoke at any time.
- The key is **never uploaded to the developer** (we operate no server). It is sent only to the LLM service you configured when a request is made (for the Google Gemini protocol, the key is sent as a request parameter, as that API requires).

## 5. Retention, security, and deletion

- **Retention**: Data stays on your device until you delete it. Log files rotate automatically and only a few recent files are kept.
- **Security**: The App runs no server and transmits nothing to the developer; local data is protected by your Windows account permissions. Communication with LLM services uses the protocol of the URL you configured (HTTPS is recommended). If you use an `http://` URL, traffic is not encrypted, so use it only on your own machine or a trusted network.
- **Deletion**: Removing a book from the library deletes its entry; translation cache can be cleared in the App; **uninstalling the App deletes all of its local data**. To delete data you previously sent to a provider, follow that provider's own procedures.

## 6. International transfers

We do not transfer your data. However, if you choose an LLM service located in another country or region, your book text will be sent to that location, which may be a cross-border transfer. Whether this occurs, and how the data is protected, depends on your choice and that provider.

## 7. Copyright and third-party information

Books may be protected by copyright and may contain personal information. You are responsible for ensuring you have the right to read and translate the book and to provide its content to the service you select.

## 8. Children's privacy

The App is not directed to children under 13 (or the higher minimum age in your jurisdiction). We do not collect personal information from anyone, including children.

## 9. Your rights

Because we hold none of your data, you can view, correct, delete, and export it yourself locally. If laws such as the GDPR, CCPA/CPRA, or China's PIPL apply to you, you have the rights they provide; since we collect no data, such requests generally require no action on our part, but please contact us with any questions.

## 10. Changes to this policy

We may update this policy. Material changes will be posted on this page and the "Effective date" updated. Continued use of the App after a new version is published means you accept the updated policy.

## 11. Contact

[Developer name]　[contact@example.com]　[optional postal address]
