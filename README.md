# txt.matthewzring.dev
This site is used to view `.txt` files that have been uploaded to Discord.
The site is static; the data loading and formatting is performed clientside.
Deleting the original file from Discord will also prevent loading it with this site.

## Example
Link to a txt file uploaded to Discord:
> https://cdn.discordapp.com/attachments/1162810075895824515/1220643987610669106/example.txt

Take the relevant substring (channel id, attachment id, and attachment name):
> 1162810075895824515/1220643987610669106/example

Add as a query parameter:
> https://txt.discord.website?txt=1162810075895824515/1220643987610669106/example

For raw (non-formatted) output, append `&raw=true`:
> https://txt.discord.website?txt=1162810075895824515/1220643987610669106/example&raw=true

## Logging format
Additional formatting will occur for lines formatted in the following way:
```
[Timestamp] Username Up To 70 Chars (optional Discord ID) : Content
```
Ex:
```
[October 29, 2018 at 5:37 PM] matthewzring (123456789012345678) : Hello there
```
