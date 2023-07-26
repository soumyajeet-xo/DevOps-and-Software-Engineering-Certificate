## File and Directory Navigation Commands
## Informational Commands
## File and Directory Navigation Commands
- ls
- ls -l (child file.. longer detailed format)
- pws (current )
- cd
- pwd

## File and Directory Management Commands
- mkdir
- rm
- rm -r (remove all subfolders)
- rm -f
- rmdir (to remove empty directories)
- touch (to create empty file)
- cp (copy)
- cp -r (recursively copy)
- chmod
- chmod +x myscript.sh

## Viewing File Content
- cat
- more (file content in a page-by-page format)
- head (first N lines)
- head -n 3
- tail (last N lines)
- wc (word count, line count, character count)
- wc -l 
- wc -w
- wc -c

## Useful Commands for Wrangling Text Files
- sort pets.txt
- sort -r pets.txt (reverse order)
- uniq pets.txt (removes repeated lines only if they are consecutive)
- grep ch people.txt  (returns matching)
- grep -i ch people.txt (case insensitive matching)
- cut -c 2-9 people (cut 2nd to 9th character from every line)
- cut -d ' ' -f2 people.txt (delimiter blank space.. thus all last name of people.txt)
- paste 
- paste first.txt last.txt yob.txt (merge)
- paste -d ',' first.txt last.txt yob.txt

## Networking Commands
-  hostname - (returns hostname of the machine)
-  hostname -i (IP address)
-  hostname -s (drop suffix)
-  ifconfig (display info regarding communication)
-  ifconfig eth0 (displays internet address, number of packets,drop packets, etc)
-  ping (send icmp packets listen for a response and prints the result)
-  ping www.google.com
-  ping -c 5 google.com
-  curl www.google.com (returns the HTML of the landing page)(transfer data to and from URL)
-  curl www.google.com -o  google.txt
-  head -n 1 google.txt
-  wget(web get) Download files from a url
-  wget example.com/path/test.txt

File Archiving and Compression Commands
- Archiving is the process of storing information that are not regularly  used but want to be preserved
- archiving make the collection more portable  
- File compression is the process of reducing the size of the file by taking advantage of redundancy
- ls -r (recursive list)
- tar -cf notes.tar notes (archive)
- tar -czf notes.tar.gz notes (archive + compress)
- tar -tf notes.tar (all the directories and files in the tar)
- tar -xf notes.tar notes (dearchive)
- tar -xzf notes.atr.gz notes (decopress)
- zip -r notes.zip notes
- 
- 
- 
-   

































