This is a list of things about the program that aren't obvious.

- The pathway view uses adbio rest api which might be out of date. The reason for using this api is because at the time(6/13/2017) kegg doesn't have support for [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Access_control_CORS)
which doesn't allow for a website to use an ajax call to another website that doesn't have the same domain. To fix this the website would
require a new backend server, maybe nodejs that would provide the necessary api to relay kegg's api. Or Kegg needs to update their api to allow for CORS. You can check the availability of bioinformatics services that support CORS [here](http://lindenb.github.io/pages/cors/index.html).
