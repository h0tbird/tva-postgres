<img src="http://45.media.tumblr.com/0370959cd51e9ffd354f8f2e825c05c3/tumblr_n6jwtyRzcU1rwdgsoo1_1280.gif"
  align="right" border="0" width="128" height="128" />

# tva-postgres

[![Build Status](https://travis-ci.org/katosys/tva-postgres.svg?branch=master)](https://travis-ci.org/katosys/tva-postgres)

Containerized PostgreSQL service.

#### Clone

Do not clone this repository.  
The control repository is named `the-voting-app`.  
Perform a recursive clone of the control repository:

```
git clone --recursive ${GIT_SERVER_URL}/the-voting-app.git
```

#### Tip

Query the `votes` table:

```
docker exec -it <docker-id> /bin/bash -c \
  "psql -U postgres -d postgres -c 'SELECT * FROM votes'"
```

Query the results:

```
docker exec -it <docker-id> /bin/bash -c \
  "psql -U postgres -d postgres -c 'SELECT vote, COUNT(id) AS count FROM votes GROUP BY vote'"
```
