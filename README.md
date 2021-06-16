# Covid-19 Confirmed Cases Visualization

This project recreates the COVID-19 growth trajectory plots using publicly available data compiled by [Johns Hopkins](https://github.com/CSSEGISandData).

### Environment

Create your python virtual environment of your choice. When that environment is active, run the following command:

​```bash
pip install -r requirements.txt
​```

### Data

The Center for Systems Science and Engineering at Johns Hopkins maintains daily summary 
of Coronavirus data around the world in a [GitHub repository](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports). 
Run the `update_data.py`script to update the data. The command below will download the
data from Jan 22 to April 25 and save it in the `data/` folder of this directory.

​```bash
python scripts/update_data.py --end 2020-04-25
​```

### Visualization

Once the data is downloaded, run the `make_plot.py` script to create an interactive 
plot of the confirmed cases by country. 

```bash
mkdir figures
python scripts/make_plot.py
```
