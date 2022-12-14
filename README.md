add-to-hosts(1) -- Add or remove a host in /etc/hosts
=============================================

## SYNOPSIS

`add-to-hosts <HOSTNAME> [<TARGET_IP>,--rm]`

## DESCRIPTION

Easier manage the /etc/hosts file.  
Does not allow aliases. But you can add them manually.  
If the host already exists in /etc/hosts, the current target hostname/IP/FQDN
will be overwritten.

## OPTIONS

* `-h`, `--help` :
  Displays the help screen.

* `--rm` :
  Remove a host from the hosts file.

## EXAMPLES

Append the host 'myserver' with the IP 192.168.1.55 to the hosts file.

    $ add-to-hosts myserver 192.168.1.55

Append the host 'myserver' with the IPs 192.168.1.55 and 192.168.1.56.

    $ add-to-hosts myserver "192.168.1.55 192.168.1.56"

Remove the host 'myserver' from the hosts file.

    $ add-to-hosts myserver --rm

## COPYRIGHT

See license file

## SEE ALSO

hosts(5)
