# Creative ideas in Google Colab

A beginner-friendly notebook that asks for an everyday object and uses the OpenAI Responses API with `gpt-6-luna` to suggest **one unusual, practical use**.

## Run the notebook

1. Open [Google Colab](https://colab.research.google.com/), choose **File → Upload notebook**, and upload `creative_ideas.ipynb`.
2. Run the installation cell to install or update the OpenAI Python SDK.
3. Run the next code cell. Enter your OpenAI API key in the hidden `getpass` prompt, then enter an everyday object such as a paper clip.
4. Read the idea. Run that cell again to try another object.

You need internet access, an OpenAI API key, access to `gpt-6-luna`, and API billing/credits. API requests may incur charges. If a request fails, check your key, model access, billing, and connection.

## Keep your key private

- Enter the key only in the hidden runtime prompt. Never paste it into source code, notebook text, output, or Git.
- The notebook keeps the key in runtime memory; it does not write it to disk or an environment file. It suppresses raw request errors to avoid exposing sensitive details.
- Disconnect and delete the Colab runtime when finished. Clear cell outputs before sharing or committing, and inspect the notebook for sensitive content.
- If a key is accidentally exposed, revoke it and create a replacement.

The notebook is provided with no saved outputs. Its Python flow was checked without making a paid API request.

See the [official OpenAI text-generation guide](https://developers.openai.com/api/docs/guides/text?lang=python) for the Responses API pattern used here.

The existing `hello_colab.ipynb` remains available as a separate coursework demo.
