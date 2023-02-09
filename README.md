# Check Free Space in Linux Partition
 These are basic command which is use to check free space in existing partition in linux OS

# Below command you can run to check free space in Linux OS



To see in TB:

# parted /dev/sda unit TB print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

To see in GB:

# parted /dev/sda unit GB print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

To see in MB:

# parted /dev/sda unit MB print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

To see in bytes:

# parted /dev/sda unit B print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

To see in %:

# parted /dev/sda unit '%' print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

To see in sectors:

# parted /dev/sda unit s print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

Change `/dev/sda` as per you Linux OS partition.
