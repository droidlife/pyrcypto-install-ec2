# pyrcypto-install-ec2
Guide for installing pycrypto pip module on amazon ec2 linux

<h2> Steps </h2>

<b>Note: </b> Activate your python virtual environment (if available)

1.  sudo yum install gcc
2.  sudo yum install make
3.  wget ftp://ftp.gmplib.org/pub/gmp-5.0.5/gmp-5.0.5.tar.bz2
4.  bunzip2 gmp-5.0.5.tar.bz2
5.  tar -vxf gmp-5.0.5.tar
6.  sudo yum install m4
7.  wget http://www.mpir.org/mpir-2.5.1.tar.bz2
8.  bunzip2 mpir-2.5.1.tar.bz2
9.  tar -vxf mpir-2.5.1.tar
10. export ac_cv_func_malloc_0_nonnull=yes ( run the command in terminal )
11. easy_install -U PyCrypto


<h2> Test PyCrypto </h2>

$ python
>>> from Crypto.Cipher import AES

If this works, you should be good to go.
