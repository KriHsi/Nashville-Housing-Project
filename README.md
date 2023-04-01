# Nashville-Housing-Project

## Dataset: Nashville Housing data
### Purpose of the exercise: using SQL to clean up raw data for analysis

#### Cleaning log: 
1.	Standardize data format, convert saledate(datetime) to saledate(date) rename as SaleDateConverted
2.	Add a new column SaleDateConverted to dataset, to include new saledate format, convert with UPDATE function
3.	Populate property address data: locate data with NULL in PropertyAddress, to determine if it can be populated with available reference data
4.	Search with ParcelID to locate reference, search result shows identical parcelID will have identical PropertyAddress, can populate with join table.
5.	Join table to fill in the NULL for PropertyAddress, join condition using ParcelID and UniqueID, display which PropertyAddress is NULL
6.	Populate ori.PropertyAddress with new.PropertyAddress to fill up the null, use ISNULL function to create a new column
7.	Update dataset with new PropertyAddress
8.	Double check if there are any nulls in PropertyAddress
9.	Separate PropertyAddress into individual columns(Address, City, State)
10.	Add two new column, PropertySplitAddress and PropertySplitCity to ori dataset
11.	Separate OwnerAddress into separate column: Address, City and State
12.	Add new column for address, city, and state into ori dataset
13.	Change Y and N to Yes and No in “SoldAsVacant” field
14.	Remove duplicate fields
15.	Delete unused columns

