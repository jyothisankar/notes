### rpms shortcuts

#### To query the size of rpms

rpm -qa --queryformat '%{SIZE} %{NAME} \n' |sort -n -r|head -10

