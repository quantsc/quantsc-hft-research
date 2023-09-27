# HFT Research with Databento
## Summary
We are analyzing market microstructure data from 2018-2023 of the top 50 and bottom 50 tickers (by volume) of the S & P 500, with the intent of using this data to predict short term price movements.  We first are conducting a literature review of market microstructure features, implementing them, and seeing how they affect the performance of a linear regression model. After reviewing the literature, we will focus on combining and modifying existing features, as well as developing unsupervised techniques for feature extraction. Once we have established a strong baseline, we will begin using more complex models for prediction. Our primary contributions are a novel demonstration of the use of DataBento data for short term predictions, and any market microstructure features that we create/identify.   

## Introductory/Related Work 
The best introduction to our problem is likely this [blog post](https://blog.headlandstech.com/2017/08/). For more specific technical questions, [quant stack exchange](https://quant.stackexchange.com/) is a good place to look, and [r/quant](https://www.reddit.com/r/quant/) can also be helpful (in my experience, much less so).  

The most widely accepted resource for Market Microstructure is Trading and Exchanges by Dr. Larry Harris. Market Microstructure in Practice is a more recent and accessible book on the subject.  Algorithmic and HFT is a good introduction to the field as a whole. You can find them all [here](https://drive.google.com/drive/folders/1vJjAp80vsVrtAmwEFCjfoozFyOie6PoW?usp=drive_link).


The prevailing wisdom in industry is that there are no good books on the subject, largely because the majority of the experts are employed by proprietary trading firms, and are not looking to publish their strategies. Despite that, most trading firms still recommend that their new researchers read Trading and Exchanges at least, among others. 


## Papers 
- [Market Microstucture: A Practitioner's Guide](http://www.chesler.us/resources/academia/microstructure_survey_madhavan.pdf)
- [Statistical Approaches for HFT  Data](https://par.nsf.gov/servlets/purl/10378098)
- [HFT in LOB](https://math.nyu.edu/~avellane/HighFrequencyTrading.pdf)
- [HFT for Price Discovery](https://faculty.haas.berkeley.edu/hender/HFT-PD.pdf)
- [ML for MM & HFT](https://www.cis.upenn.edu/~mkearns/papers/KearnsNevmyvakaHFTRiskBooks.pdf)
- [Market Microstructure for HFT](https://statmath.wu.ac.at/~hauser/LVs/FinEtricsQF/References/oHara2015JFinEco_HighFrequ_Market_MiicroStruct.pdf)
