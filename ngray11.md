
# URL Shortener

The program will take any URL and shortened it to the desired length or text. This solves the problem of egregiously long URLS when sharing or storing links.
The ability to shorten URLs is an important tool to share links, especially if there is a character limit per message.
The program will also provide fast lookups to ensure minimal redirection time for a smooth experience and customization for short URLs.

# Technologies

1. The URL Shortener will require a third party server to store shortened URLs. Users can create a custom URL which will be stored in the database. Any of these URLs will direct to the server, then paired with the long URL and redirected to the webpage.
1. A cache will also be present for frequently visited URLs. The purpose of which is to reduce queries to the server for a faster experience.
1. An expiration date for the shortened URL is given, which the user can change to limit access for the receiver.
1. epoll will be used to monitor network sockets to limit overhead.
1. A write ahead log will record URLs before official creation to avoid waiting for disk writing.
1. Containerization to efficiently run requests.

# Features

1. Expanding on the custom URL, users can write any string. However, some characters will be restricted, such as '/', as to not cause any failures.
1. The program will provide analytics to monitor interactions with URLS.
1. An interface to view and look up existing URLs.
1. 
