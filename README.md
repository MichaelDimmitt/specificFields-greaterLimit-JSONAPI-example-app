## Larger responses from network requests.

## GraphQL should give more results if there is a low quota
1) When a company has extensive validation.
<br/> Fields that are a finite length example: 50 characters. 
<br/> Get a more favorable worstcase rating than Description 400 characters.

2) If every field had a character quota, queries could be completed via worst case.

3) If the user is requesting 3, 50 character fields as the entire response.
<br/> They should be able to query a larger limit.


## specificFields-greaterLimit-JSONAPI-example-app

## Most Ideal Situation:
1) Everything is queried on the server...
<br/>tries to return the entire response. 
<br/>However, if the response is above the space requirements of 1MB.
<br/>Pagination is done backwards to shrink the response.
<br/>When the response meets space requirements the response is sent to the client.
<br/>Appended with how many records are left.

## Option 2: 
2) for certian fields that will always return one line,
<br/>if those fields are present calculate number of lines possible.
<br/>we are good as long as it is below that number of lines example 3000 lines.

## Option 3: 
3) num chars are figured out for the response and limit is done by number of characters

