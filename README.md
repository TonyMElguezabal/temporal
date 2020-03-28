# temporal
ssh-keygen -t rsa -b 4096 -C jose.elguezabal@gmail.com

# Generate public ssh key
ssh-keygen -y -f ~/.ssh/id_rsa > ~/.ssh/id_rsa.pub

# 3 Add key to shh
eval "$(ssh-agent -s)"

# 4 Add ssh key to the system
ssh-add ~/.ssh/id_rsa


