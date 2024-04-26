# Leveraging Machine Learning for Algorithmic Trading
This repository houses the code for an AI-powered trading bot. The bot leverages machine learning for sentiment analysis to inform trading decisions.

Here's what you'll find:

* A step-by-step breakdown of the bot's creation process, including building the baseline block, defining a trading strategy, setting up backtesting, and integrating a sentiment analysis model.
* Code utilizing libraries like Lumot, Yahoo Finance, and Alpaca for data acquisition and trading functionality.
* Exploration of machine learning integration through sentiment analysis of news articles to influence buy and sell signals.

**Important Note:** *This project is for educational purposes and focuses on paper trading. Live trading involves real-world risks and fees not accounted for here.*

This repository provides valuable insights for developers interested in building AI-powered trading bots and exploring the intersection of machine learning and algorithmic trading.

# Startup
1. Create a virtual environment `conda create -n trader python=3.10` 
2. Activate it `conda activate trader`
3. Install initial deps `pip install lumibot timedelta alpaca-trade-api==3.1.1`
4. Install transformers and friends `pip install torch torchvision torchaudio transformers` 
5. Update the `API_KEY` and `API_SECRET` with values from your Alpaca account 
6. Run the bot `python tradingbot.py`

<p>N.B. Torch installation instructions will vary depending on your operating system and hardware. See here for more: 
<a href="pytorch.org/">PyTorch Installation Instructions</a></p>

If you're getting an SSL error when you attempt to call out to the Alpaca Trading api, you'll need to install the required SSL certificates into your machine.
1. Download the following intermediate SSL Certificates, these are required to communicate with Alpaca
* https://letsencrypt.org/certs/lets-encrypt-r3.pem 
* https://letsencrypt.org/certs/isrg-root-x1-cross-signed.pem 
2. Once downloaded, change the file extension of each file to `.cer` 
3. Double click the file and run through the wizard to install it, use all of the default selections. 

</br>
# Other References

<p>-<a href="github.com/Lumiwealth/lumibot)">Lumibot</a>:trading bot library, makes lifecycle stuff easier .</p>

# Who, When, Why?

👨🏾‍💻 Author: Usama Buttar <br />
📅 Version: 1.x<br />
📜 License: This project is licensed under the MIT License </br>
