# Nifty Returns Vizualizer
 A D3.js Swarmplot implementation to vizualize the Nifty-X Month-To-Date(MTD) returns.
 Based on Chartfleau's Viz. for the S&P500 https://github.com/janvarsa/D3-Swarm-Tutorial / https://www.chartfleau.com/tutorials/d3swarm

 * Month-To-Date Returns: MTD is a period starting at the beginning of the current calendar month and ending at the current date.  
 For example: the month to date return for the stock is 8%. This means from the beginning of the current month until the current date, stock has appreciated by 8%. [source:wikipedia](https://en.wikipedia.org/wiki/Month-to-date)

 * Data requirements: A Time/Date sorted CSV with the following fields for each stock
   * Date
   * Ticker: The stock's name/trading Ticker.
   * Sector: The stock's operating sector/domain.
   * Close: The stock's daily closing price.
   * Market Cap[optional]: The stock's market cap.
   * Return: Derived field(from either the ratio of current day's close wrt starting day's close or the ratio of the Market Cap on the two days)

# Getting Started
 For the D3 module to be able to read the csv, a local http server needs to be running.
 Easiest way (node.js already installed)
 * npm install --global http-server
 * run the command: http-server, in the project dir.
 * Browse to http://localhost:8080/main.html 
