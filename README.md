# wiki-graph

Utilizes wiki API to build a edge and node files for graph of wikipedia page links for use in IBM's System-G

---

### System-G
[System-G](http://systemg.research.ibm.com/) is IBM's graph database for search and querying graphical relationships. For batch loading, it takes as input two files, a node file and an edge file.

---

### wikipedia API for python:

The [Wikipedia API](https://pypi.python.org/pypi/wikipedia/) for python contains functions which obtains information about a particular wikipedia page and its relations to other pages.

---

### content:

The goal is to utilize the wikipedia API to build a graph database. To do this, **wiki-edge.py** takes as input a wikipedia page title and discovers other pages that are linked by the first page. The process is repeated *k* times, for a longest acyclic subtree to no longer than *k* nodes. **format.py** is trivial in reformatting ascii to unicode before I found a better way to do it.

