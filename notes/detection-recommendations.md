# Detection Recommendations

## Risky Protocols to Monitor

- TELNET
- FTP
- POP3
- HTTP authentication
- Unencrypted SMTP

## Recommendations

- Disable TELNET where possible.
- Replace FTP with SFTP or SCP.
- Use HTTPS instead of HTTP.
- Alert on cleartext login attempts.
- Monitor unexpected file transfers.
- Review PCAPs during incident response.

## Example Detection Logic

Alert when internal systems use TELNET:

```text
protocol == telnet
