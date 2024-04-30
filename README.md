# Free-GPT4-WEB-API (Sebu's special version)

FreeGPT4-WEB-API is a python server that allows you to have a self-hosted GPT-4 Unlimited and Free WEB API, via the latest Bing's AI.

<details>
<summary>GUI Preview:</summary>
<img src="./img/login.png" width="408" height="290" />
<img src="./img/settings.png" width="408" height="290" />
</details>

## Installation

To install the required libraries, you can use the following command:

`pip3 install -r requirements.txt`

## Usage

You only have one Python file, so shouldn't be that hard.
It is buildt with flask, so in the terminal you will have a link to open your browser. Then you can edit the url by adding `?text=your request here`

To run the server, use the following command:

```shell
python3 FreeGPT4_Server.py [-h] [--remove-sources] [--enable-gui]
                           [--private-mode] [--enable-history] [--password PASSWORD]
                           [--cookie-file COOKIE_FILE] [--file-input] [--port PORT]
                           [--model MODEL] [--provider PROVIDER] [--keyword KEYWORD]
                           [--system-prompt SYSTEM_PROMPT]
```

Options:

`-h, --help` show this help message and exit

`--remove-sources` Remove the sources from the response

`--enable-gui` Use a graphical interface for settings

`--private-mode` Use a private token to access the API

`--enable-history` Enable the history of the messages

`--password PASSWORD` Optional, set a password for the settings page [mandatory in docker envirtonment]

`--cookie-file COOKIE_FILE`
Use a cookie file

`--file-input` Add the file as input support

`--port PORT` Change the port (default: 5500)

`--model MODEL` Change the model (default: gpt-4)

`--provider PROVIDER` Change the provider (default: Bing)

`--keyword KEYWORD` Add the keyword support

`--system-prompt SYSTEM_PROMPT`
Use a system prompt to 'customize' the answers

## Configuration

The server can be configured by editing the `FreeGPT4_Server.py` file. You can change the server's port, host, and other settings. Please do _not_ edit the `settings.json` file manually, use the GUI or the corresponding parameters. The only cookie needed for the Bing model is _"\_U"_.

## Star History

Comming soon!

## Notes

- The demo server may be overloaded and not always work as expected. (Check the "Demo Server Status" above)
- Any kind of contribution to the repository is welcome.

## Todo ✔️

- [x] Fix Demo Server
- [x] Update README
- [ ] add my own Star history
- [ ] remove unused stuff
