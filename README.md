# showing-the-code-snippet-for-LIST-ALL-test-case
def test_list_all_products(self):
    # Send a GET request to list all products
    response = self.client.get("/products")
    
    # Assert the response status and content
    assert response.status_code == 200
    assert isinstance(response.json, list)
