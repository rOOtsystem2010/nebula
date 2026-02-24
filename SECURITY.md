Hi,

I have discovered a critical command injection vulnerability in your repository berylliumsec/nebula in the file src/nebula/tools/terminal.py, specifically at line 23 where user-supplied input is executed via subprocess.check_output with shell=True. This allows arbitrary command execution by any user who can pass input to this function.

Recommendation: Avoid using shell=True with untrusted input. Instead, sanitize input or avoid shell execution where possible.

Please let me know if you need further details, and let me know when it’s safe to disclose further.

Best regards,

Helmi
https://github.com/rOOtsystem2010
