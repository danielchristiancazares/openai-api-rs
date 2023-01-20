# openai-api-rs
This Rust application uses OpenAI's API to fine-tune a code generation model. It takes in a dataset file and a model name, and trains the model on the provided dataset. Once the model is fine-tuned, it can be used to generate code. The app utilizes concurrency to process the dataset file faster and also uses a configuration struct to centralize the API key, model name, and dataset. It also uses the `davinci-003` engine, but it can be changed to use any model.

## Installation

To use this application, you will need to have [Rust](https://www.rust-lang.org/tools/install) installed on your machine.

You will also need to have an API key for OpenAI, which can be obtained [here](https://beta.openai.com/account/api-keys).

Once you have Rust and an API key, you can clone this repository and run the following command to install the dependencies:

```
cargo install
```

## Usage

To use this application, you will need to provide a dataset file and a model name. The dataset file should be a text file containing the code you want to use to train the model.

You will also need to set the environment variable `OPENAI_API_KEY` to your OpenAI API key.

Then, you can run the following command to fine-tune the model and generate code:

```
cargo run -- dataset_file.txt model_name
```


You can also change the engine used, by default it is set to 'davinci-003' but it can be changed to use the latest one.

## Contributing

If you would like to contribute to this project, please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
