# wikidata_detail

To achieve **Keyword Frequency Analysis** and **Tag Validation against Wikidata** we make great efforts on this.

In the detail, at first, we count the keyword in every dataset and get a list of PID. Next, we send api to wikidata to get the corresponding name in wikidata.

The api is liked this: 
https://www.wikidata.org/wiki/Special:EntityData/{i}.json

In the context of our analysis, we undertake a comparison to determine whether the most frequently used tags correspond to Wikidata keywords. We leverage the wikidataintegrator library, employing the **sparql_query** functionality. However, it's important to note that this library primarily recognizes English language inputs. Yet, Wikidata keywords may include Chinese. To address this linguistic diversity, we adopt a strategy based on the initial character of the returned keyword.

We achieve this by utilizing **ASCII codes** to differentiate between English, Chinese, and numeric keywords. If a keyword starts with a numeric character, we approach the search process comprehensively. Specifically, we explore results in both English and Chinese to ensure a comprehensive coverage of relevant data. This approach is implemented selectively to optimize the efficiency of our search procedure.

Finally, we return the words which are in the wikidata or not. **重複出現** means it has been built in wikidata, **需要補充** means the page for the words hasn't been built in the wikidata.