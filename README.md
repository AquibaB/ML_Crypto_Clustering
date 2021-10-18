# project_2

This project focused on the use of unsupervised learning techniques to glean insights into the price action of different cryptocurrencies, as measured by daily changes in their respective market capitalizations. Additionally, we performed sentiment analysis on news headlines and explored their relationship with price movements.

The technologies utilized included the CoinGecko API, hvplot, sklearn, holoviews, pandas, and matplotlib. Specifically, we leveraged clustering analysis, covariance, and manifold estimation for the price analysis, and manual coding, kmeans, and hvplot for the news analysis. JupyterLab was used to prepare the data. For additional versatility, we also saved the code in Google Colab.

Installations required include hvplot, sklearn, matplotlib, and pycoingecko. All installs can be completed through !pip install.

Price data was collected from pycoingecko and put into a Pandas DataFrame. For the news analysis, the manual sentiment coding that was performed in Excel was added to the DataFrame. In total, 52 cryptocurrencies were analyzed, along with 64 news events. Preprocessing was done using MinMaxScaler.

For the price analysis, a three-model cluster was developed, utilizing graphical lasso, affinity propagation, and locally linear embedding. The results are shown here:
![image](https://user-images.githubusercontent.com/85848524/137645319-c61f37e4-65a8-412d-bf9e-de395e4ecf40.png)

There are some logical relationships, such as clustering and bold lines between DEX platforms (e.g. Sushiswap, Uniswap) and smart contract platforms. Others are less correlated than might be expected, such as between bitcoin and ethereum.

For the news analysis, binary manual coding indicating sentiment (-1 for negative, +1 for positive) was done across several subjects - institutional news, China news, regulatory news, and overall sentiment:
![image](https://user-images.githubusercontent.com/85848524/137645682-e13d72ac-e544-4409-b0fe-46fb125a84d4.png)

An example is shown below, using the China news scatter plots to indicate that DEXs outperformed other tokens on days when there was China-related crypto news:
![image](https://user-images.githubusercontent.com/85848524/137645744-58c22ccb-7e0e-48bb-b574-222d0c06dff7.png)

For institutional news, large-cap tokens tended to react more negatively:
![image](https://user-images.githubusercontent.com/85848524/137645796-8d873e3b-2f61-43eb-b6b4-4da2e5e44e33.png)

The conclusions of the project are summarized below:
![image](https://user-images.githubusercontent.com/85848524/137646412-b5323670-6b25-4769-9cb4-1f5c342ce83a.png)


Link to MC_Analysis on Google Colab: https://colab.research.google.com/drive/1zVg8wN15cCza-Al0l8htWiwsxV0yU4Zx?usp=sharing
