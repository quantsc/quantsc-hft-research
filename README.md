# HFT Research with Databento
## Summary
We are analyzing market microstructure data from 2018-2023 of the top 50 and bottom 50 tickers (by volume) of the S & P 500, with the intent of using this data to predict short term price movements.  We first are conducting a literature review of market microstructure features, implementing them, and seeing how they affect the performance of a linear regression model. After reviewing the literature, we will focus on combining and modifying existing features, as well as developing unsupervised techniques for feature extraction. Once we have established a strong baseline, we will begin using more complex models for prediction. Our primary contributions are a novel demonstration of the use of DataBento data for short term predictions, and any market microstructure features that we create/identify.   

## Introductory/Related Work 
The best introduction to our problem is likely this [blog post](https://blog.headlandstech.com/2017/08/). For more specific technical questions, [quant stack exchange](https://quant.stackexchange.com/) is a good place to look, and [r/quant](https://www.reddit.com/r/quant/) can also be helpful (in my experience, much less so).  

The most widely accepted resource for Market Microstructure is Trading and Exchanges by Dr. Larry Harris. Market Microstructure in Practice is a more recent and accessible book on the subject.  Algorithmic and HFT is a good introduction to the field as a whole. You can find them all [here](https://drive.google.com/drive/folders/1vJjAp80vsVrtAmwEFCjfoozFyOie6PoW?usp=drive_link).

The prevailing wisdom in industry is that there are no good books on the subject, largely because the majority of the experts are employed by proprietary trading firms, and are not looking to publish their strategies. Despite that, most trading firms still recommend that their new researchers read Trading and Exchanges at least, among others. 

## Project Breakdown 
The initial steps are as follows: 
- Pull the data from Databento, organize it so that it is easy to work with
- Review the literature, try to find as many features as possible for short term price prediction
    - If you find a novel feature, put the paper in Resources/Papers.md with a short (1-3 sentence) description of the feature. Ideally, add a function to implement it on the databento data 
    - If you find an interesting paper related to feature construction/signal extraction, also put it in Papers.md
- Identify the best modeling techniques that are robust to noise/distributional shifts.
    - Again, add any relevant papers to papers.md with a short synopsis.
- After extracting signals and correctly predicting price movements, we need to identify trading rules. A (non-exhaustive) list of things to consider:
    - How confident are we in out price movement?
    - With the transaction cost, is it worth it?
    - How can we account for adverse selection?
    - Can we identify correlated price movements for arbitrage?
    - Are there patterns related to time of day?
    - How does the signal perform on highly liquid vs highly illiquid stocks?
