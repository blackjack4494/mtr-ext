original https://github.com/traviscross/mtr

mtr-ext

Ubuntu18.04  
(I do not know if it's mandatory to install everything - need to sort it out later)  

git clone https://github.com/blackjack4494/mtr-ext.git  
cd mtr-ext/  

chmod +x bootstrap.sh  
chmod +x build-aux/git-version-gen  
chmod +x build-aux/mangen.sh  

apt update && apt upgrade  
apt install build-essential  
apt install autotools-dev  
apt install automake  
apt install autoconf  
apt install autoheader  
apt install pkgconf  
apt install libncurses-dev  
apt install ncurses-dev  

./bootstrap.sh  
./configure  
make  

Sample Output  
with 'standard' setting  
https://gist.github.com/blackjack4494/b54ccb55502a3e4d7c04c112188f4048  


Where I changed the output    
https://github.com/blackjack4494/mtr-ext/blob/master/ui/split.c#L106-L120  

What the output means  
https://github.com/blackjack4494/mtr-ext/blob/master/ui/mtr.c#L75-L91  
