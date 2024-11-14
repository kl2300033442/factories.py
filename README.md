Feature: Product Management

  Scenario: Updating a Product
    Given a product with ID "123" exists
    When I update the product with new details:
      | name        | New Product Name |
      | price       | 49.99            |
      | description | Updated details  |
    Then the product should have the updated details
