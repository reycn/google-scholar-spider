# Google Scholar Spider Documentation

Google Scholar Spider is a Python-based tool that retrieves data on articles published on Google Scholar based on given keywords. It allows users to save results as CSV files, plot results, and filter results by year and citation count.

## Usage

The Google Scholar Spider can be used by running the `google_scholar_spider` function from the command line and passing in any required parameters.Available parameters include: 

- \*\*kw &lt;keyword&gt; (default "machine learning") The keyword to search for. 
- \*\*nresults &lt;number of results&gt; (default 50) The number of articles to be searched on Google Scholar. --\*\*notsavecsv Use this flag to print results without saving them to a CSV file. 
- \*\*csvpath &lt;path&gt; The path to save the exported CSV file. Defaults to the current folder. 
- \*\*sortby &lt;column&gt; (default "Citations") Sorts data by column. To sort by citations per year, use -- sortby "cit/year". 
- \*\*plotresults Use this flag to plot results with raw rankings on the x-axis and citation counts on the y-axis. 
- \*\*startyear &lt;year&gt; The starting year of the search article. 
- \*\*endyear &lt;year&gt; (default current year) The end year of the search article. 
- \*\*debug Use this flag to enable debug mode. Debug mode is used for unit testing and storing pages in the web archive.Examples

```
python google_scholar_spider.py --kw "deep learning" --nresults 30 --csvpath "./data" --sortby "cit/year" --plotresults 1
```

This command searches Google Scholar for articles related to "deep learning", retrieves 30 results, saves the results to a CSV file in the ". /data" folder, sorts the data by the number of citations per year, and plots the results.

## License

Google Scholar Spider is released under the MIT license.