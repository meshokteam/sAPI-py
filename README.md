# sAPI-py
Python библиотека для использования API для продавцов аукциона Мешок

```Python
# Instantiate the MeshokAPI class with your token
api = MeshokAPI('your_token_here')

# Get the list of items
item_list = api.getItemList()
print(item_list)

# Get the list of finished items
finished_item_list = api.getFinishedItemList()
print(finished_item_list)

# Get the list of unsold finished items
unsold_finished_item_list = api.getUnsoldFinishedItemList()
print(unsold_finished_item_list)

# Get the list of sold finished items
sold_finished_item_list = api.getSoldFinishedItemList()
print(sold_finished_item_list)

# Get the information of a specific item
item_info = api.getItemInfo('item_id_here')
print(item_info)

# Get the account information
account_info = api.getAccountInfo()
print(account_info)

# Get the list of common descriptions
common_description_list = api.getCommonDescriptionList()
print(common_description_list)

# Get the subcategory information
subcategory_info = api.getSubCategory('subcategory_id_here')
print(subcategory_info)

# Get the category information
category_info = api.getCategoryInfo('category_id_here')
print(category_info)

# Get the list of currencies
currency_list = api.getCurencyList()
print(currency_list)

# Get the list of countries
country_list = api.getCountryList()
print(country_list)

# Get the list of cities for a specific country
cities_list = api.getCitiesList('country_id_here')
print(cities_list)

# Stop the sale of a specific item
stop_sale_response = api.stopSale('item_id_here')
print(stop_sale_response)

# Relist a specific item
relist_item_response = api.relistItem('item_id_here')
print(relist_item_response)

# Delete a specific item
delete_item_response = api.deleteItem('item_id_here')
print(delete_item_response)

# List a new item
new_item_params = {

    #Add params
}
list_item_response = api.listItem(new_item_params)
print(list_item_response)

# Update an existing item
update_item_params = {
    'id': 'item_id_here',
    #Params
}
update_item_response = api.updateItem(update_item_params)
print(update_item_response)
```
