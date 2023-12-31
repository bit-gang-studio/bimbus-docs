<body>
    <div align="center">
        <h1 align="center">
            <img src="https://raw.githubusercontent.com/bitgangstudio/bimbus-cli/master/icons/bgs.png" width="45" />
            <img src="https://raw.githubusercontent.com/bitgangstudio/bimbus-cli/master/icons/bimbus.png" width="45" />
            <img src="https://raw.githubusercontent.com/bitgangstudio/bimbus-cli/master/icons/openai.png" width="45" />
            <br/>
            <span>BimBus AI <small>[Simple Docs]</small></span>
        </h1>
        <h3><strong>Automated Code Documentation</strong></h3>
        <p><strong>Developed using OpenAI's GPT language model APIs</strong></p>
        <p align="center">
            <img src="https://img.shields.io/badge/Markdown-000000.svg?stylee&logo=Markdown&logoColor=white" alt="Markdown" />
            <img src="https://img.shields.io/badge/Node.js-339933.svg?style=flat&logo=node.js&logoColor=white" alt="Node JS" />
            <img src="https://img.shields.io/badge/npm-CB3837.svg?style=flat&logo=npm&logoColor=white" alt="NPM" />
            <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
        </p>
    </div>
</body>

📖  Overview
-------------------

Automatically Document Programming Files and Scripts with BimBus. BimBus is a sleek and powerful command line tool crafted with Node.js and fueled by OpenAI's cutting-edge technology. Effortlessly generate thorough and comprehensive documentation for your code files. Works for all file types and projects.

⚙️  System Requirements
-------------------

*   Node.js (v16 or higher)
*   npm (v8 or higher)

🚀  Installation
------------

```
 $ git clone https://github.com/bitgangstudio/bimbus-cli.git
 $ cd bimbus-cli
 $ npm install
 $ npm run build
```

💻  OpenAI API
------------

To use BimBus AI, you will need to create an account with OpenAI to generate an API key. The steps below outline this setup process:

1. Go to the [OpenAI website](https://platform.openai.com/).
2. Click the "Sign up for free" button.
3. Fill out the registration form with your information and agree to the terms of service.
4. Once logged in, click on the "API" tab.
5. Follow the instructions to create a new API key.
6. Copy the API key and keep it in a secure place.

📝  Usage
-----

To generate documentation using BimBus, run the following command:
```
 $ node dist/index.js -t <openai_access_token> \
                      -i <input_file_path> \
                      -m <model> \
                      [-o <output_file_directory>] \
                      [-f <filetype>] \
                      [-v] [-k] [-h]
```
The command accepts the following arguments:

*   `-t` or `--token`: Specifies the OpenAI Access Token.
*   `-i` or `--input`: Specifies the path to the input file containing code to generate documentation for.
*   `-m` or `--model`: Open AI Model used to process documentation. Accepts gpt-3.5-turbo or gpt-4. Default model is gpt-3.5-turbo.
*   `-o` or `--output` (optional): Specifies the output directory where the generated documentation will be saved. If not provided, the documentation will be saved in the current working directory.
*   `-f` or `--filetype` (optional): Specifies the output file type for the generated documentation (default: markdown). Can be 'markdown' or 'html'
*   `-k` or `--keep` (optional): Specifies if we should keep the meta/processing files being used as part of documentation generation process.
*   `-v` or `--verbose` (optional): Enables verbose output for detailed information (default: false).
*   `-h` or `--help`: Displays the help message for BimBus.

🌟  Examples
--------

The following are some examples on how to run BimBus.

Basic usage:
```
 $ node dist/index.js -t <OpenAI Access Token> -i path/to/file.js
```

Specifying an output directory:
```
 $ node dist/index.js -t <OpenAI Access Token> -i path/to/file.py -o output/docs/
```

Customizing the output file type:
```
 $ node dist/index.js -t <OpenAI Access Token> -i path/to/file.ts -f html
```

Enabling verbose output:
```
 $ node dist/index.js -t <OpenAI Access Token> -i path/to/file.py -v
```

Displaying help message:
```
 $ node dist/index.js --help
```

🤝  Contributions and Issues
------------------------

We welcome contributions and feedback! If you encounter any issues or have suggestions for improvements, please submit them in the [Issue Tracker](https://github.com/bitgangstudio/bimbus-cli/issues). Pull requests are also welcome.

📄  License
-------

BimBus is released under the [MIT License](https://raw.githubusercontent.com/bitgangstudio/bimbus-cli/master/LICENSE).

👩‍💻 Happy documenting with BimBus!
