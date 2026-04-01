# Exploratory analysis of bidding patterns in online auctions

## Project overview
This project is a preliminary exploration of how data from digital auction platforms can be used to understand bidder behavior. As traditional auction houses increasingly move toward hybrid and digital models, there is an opportunity to use granular transaction data to support specialists in their valuation and cataloging processes. 

The goal is not to replace the expert’s "eye," but to see if we can identify recurring patterns in the "bid-stream" that might help predict interest levels or optimal starting prices.

## The data
The analysis uses a historical dataset of bidding activity from eBay, specifically focused on items that sit between the luxury and collectible markets (e.g., Cartier and Swarovski). 

The datasets are from a companion website for the book *Modeling Online Auctions*, by Wolfgang Jank and Galit Shmueli (Wiley and Sons, ISBN: 978-0-470-47565-2, July 2010).  

* **Context:** While eBay is a high-volume platform, it provides a high-resolution look at how bidders react to price and time-principles that are often universal across different auction formats.  
* **Scope:** The dataset includes opening bids, individual bid increments, bidder reputation scores, and the final hammer price.

## Areas of exploration
My focus during this project is to look at three specific possibilities for data-driven insights:

1. **Temporal behavior (Sniping):** Identifying what percentage of activity happens in the final minutes of a sale.  Understanding this "climax" can help an auction house decide if they should implement features like "soft-closes" or "dynamic endings."

2.  **Price discovery and estimates:** Examining the relationship between the starting bid and the final result. I wanted to see if lower opening prices consistently lead to more "bidding wars" compared to starting closer to a fair market  

3.  **Bidder engagement:** Using bidder reputation scores as a proxy for experience. This helps in understanding if a specific category is attracting seasoned collectors or new, casual buyers.

## Reflection
[...]


## Installation

Clone the repo and install dependencies:  
`git clone https://github.com/IreneGrisenti/Online_Auction_Analysis.git`

Create and activate virtual environment:  
`python -m venv .venv`

Windows PowerShell:  
`.venv\Scripts\Activate`

macOS/Linux:  
`source .venv/bin/activate`

Install dependencies:  
`cd Online_Auction_Analysis python -m pip install -r requirements.txt`

## Environment

Python: 3.12.3  
Packages: Numpy, Pandas, Matplotlib, Jupyter (see requirements.txt)