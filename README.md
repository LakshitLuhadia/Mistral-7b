# Mistral-7b
This is a simple guide on how to use mistral-7b on Raspberry Pi 4 using Ollama.

I followed these steps to set-up a personal chatbot on my Raspberry Pi 4. Since it is places on my local machine, there are no data privacy concerns.

It assumes one knows how to set-up Raspberry Pi 4.

## Ollama on Linux

Install Ollama by running this one-liner:

```

curl https://ollama.ai/install.sh | sh

```

*** For manual installation, refer to: [Ollama Github Repository](https://github.com/jmorganca/ollama/blob/main/docs/linux.md) ***

Ideally, this should install Ollama on your linux system.
For any issues or updates, refer to: [Ollama Github Repository](https://github.com/jmorganca/ollama/tree/main)

## LLM on Command Line

Feel free to visit [Ollama library](https://ollama.ai/library) to pick an LLM you would want to use.
Just keep in mind that on a Raspberry Pi with 8GB RAM, you cannot use anything bigger than 7B.
Naturally, a larger model produces a slower output with more accurate responses.

For this repository, I will be using Mistral-7b.

To run Mistral on the command line, run:

```

ollama run mistral

```

Once it is successful, you will get a prompt to write your question. Ask your Question and wait for the answer :)

## Drawbacks

- When I tried running it, this worked extremely slowly. To circumvent this, you can try using a smaller LLM. Although the answers wont be quite the best, it should work faster.
- Since we are running a pre-made LLM, it naturally inherits the drawbacks of the LLM you chose.

## References

- [Ollama Github Repository](https://github.com/jmorganca/ollama/tree/main)
- [Mistral Github](https://github.com/mistralai/)
- [Running Local LLMs and VLMs on the Raspberry Pi](https://towardsdatascience.com/running-local-llms-and-vlms-on-the-raspberry-pi-57bd0059c41a)
- [Ollama Homepage](https://ollama.ai/)
- [Mistral Homepage](https://mistral.ai/)


## License

This project is licensed under the MIT License.
