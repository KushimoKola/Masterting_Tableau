### Bypassing cache and getting live data from source
- Press `F5` or selecting yout data source from `Data` and selecting `Referesh`

## Tip
- Consider using color `blind-safe colors` in your visualizations. `Orange and blue` are usually considered a color blind-safe alternative to red and green. 
- Tableau also includes a discrete color blind-safe palette. 
- Additionally, consider adjusting the intensity of the colors, using labels or different visualizations to make your visualizations more accessible.

## Working with Extracts
- An extract file contains data extracted from the source.
- There are a couple of security considerations to keep in mind when using an extract. 
 - - First, any security layers that limit which data can be accessed according to the credentials used will not be effective after the extract is created. An extract does not require a username or password. All data in an extract can be read by anyone. 
 - - Second, any data for visible (non-hidden) fields contained in an extract file (.hyper or .tde), or an extract contained in a packaged workbook (.twbx), can be accessed even if the data is not shown in the visualization. 