# OtoMoto
OtoMoto - Price Prediction

Author: Małgorzata Stolarska
E-mail address: malgorzata.stolarska@gmail.com

Purpose:
Building a model to predict car prices and classify prices as overstated, understated or average.
Model learning will be performed on the data from the website https://www.otomoto.pl/, obtained by web scrapping. The source code, that was used to retrieve the data, is in the notebook: OtoMoto - WebScrapping.ipynb.

Assumptions:
The model will be predict prices in PLN for new and used cars, but not for damaged cars.

Data description:
The Polish names of columns correspond to the fields on the otomoto.pl website. The scope of the fields varies from offer to offer and may change over time. The fields required for the model are listed at the end of the document and any additional fields will be ignored.

In addition to the columns mentioned above, the dataset includes columns:

href: link to the offer on the website (notice: it becomes inactive after the offer expires),
price_evaluation: indicates whether the car's price is in the mid-range, above or below (the value corresponds to the icon on the website); not used in price prediction but it is the basis for classification,
price: price of car,
currency: only PLN supported (offers in other currencies should be removed from the data)
price_details: additional information regarding the price, e.g. whether the price is negotiable,
seller_type: offer from a private person or from a dealer,
seller_name: field not used in price prediction.
The data used to analyze and build the model was valid on February 9, 2021.
