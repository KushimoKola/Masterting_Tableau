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

 ## Sets and Groups
 - `Group` is a combination of values from one or more dimensions. For example, with the four regions Central, East, South, and West, you might choose to create two groups: East-Central and South-West
 - `Set` is a collection of records from the data source. At a row level, each record is either in or out of the set.
### Types of Sets
 - Dynamic sets: This is computed for a single dimension based on a conditional calculation you define. As the data changes, the results of the condition may change and records may switch between in and out of the set.
 - Fixed sets: This is a list of values for one or more dimensions. If the values for a single record match the list defined by the set, then the record is in the set, and out otherwise.

 ## Filtering
 - Discrete (Blue) Fields: When filtering using a discrete field, you will be given options for selecting individual values to `keep` or `exclude`.
 - Continous (Green) Fields: 
 - - If you drop a continuous dimension onto the Filters shelf, you’ll get a different set of options.
 - - Once you’ve made a selection (or if the selection wasn’t applicable for the field selected), you will be given another interface for setting the actual filter.
 ### NOTE
 Ascertaining if a field is discrete or continous can be challenging. However, one should always think about whether they are using the field as a dimension filter or a measure filter to understand what kind of results they will get based on the order of operations.
 Important to note that: 
 - Dimension filters will filter detail rows of data.
 - Measure filters will filter aggregate rows of data at the level of detail defined by the dimensions included in your view.

