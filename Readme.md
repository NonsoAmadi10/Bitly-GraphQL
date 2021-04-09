# Bitly-GraphQL

A graphql implementation of a URL link shortener in django.

## Technologies Used

- Python 3.7+
- Django
- Graphene
- SQLite3

## Getting Started
- You will need to create a virtualenv before starting
    - Simply run:
        - `pip install virtualenv`
        - `virtualenv<name-of-your-env>`
        - `source <name-of-your-env>/bin/activate`

- Then Install the dependencies in the `requirements.txt` file using:
      - `pip install -r requirements.txt` 
- Start the server using:
        - `python manage.py runserver`
- Open your browser on the route path `/graphql`
  
- Make a graphql query using:
  > query {
   urls{
   id
    fullUrl
    urlHash
    clicks
    createdAt
        }
     }

- Make a graphql mutations using:
  
  > mutation {
  createUrl(fullUrl:"not_valid_url"){
    url {
      id
      fullUrl
      urlHash
      clicks
      createdAt
    }
  }
}


## Author
- Chinonso Amadi

Acknowledgements
  
- Digital Ocean
