### Hello, I'm Jack! 🙋🏼‍♂️

```powershell
# My domain
$domain = "itsjack.cloud"

# Define short profile introduction
function Show-Introduction {
    # Details used to build the output message
    $name       = "Jack"
    $role       = "Platform Engineer"
    $employer   = "Littlefish"
    $traits     = @("curious problem solver", "automation advocate", "always learning")
    $focus      = "deliver business value faster and more securely"

    # Use a here-string to keep my introduction readable over multiple lines
    return @"
Hello!👋🏼 I'm $name, a $role currently working at $employer.
I would describe myself as a $($traits[0]), an $($traits[1]) and someone who is $($traits[2]).
I enjoy working with teams and leveraging technology to $focus.
"@
}

# Output introduction
Show-Introduction

# See my site
Start-Process "https://hello.$domain"

# Send me an email
Start-Process "mailto:jack@$domain"
```
