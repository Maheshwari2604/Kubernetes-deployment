# Kubernetes-deployment
make containers and deploy bash , python and go language programs



mkdir code 

cd code



vi hello.sh
# bash file

#	echo 'hey bash'
#	sleep 2
#	echo 'hey python'

docker run -it --name test1 /root/code:/code alpine sh /code/hello.sh



vi hello.py
# Python file

#	#import time
#	print('hey bash') 
#	time.sleep(2) 
#	print('hey python')
#	time.sleep(2)
#	print(time.ctime())

docker run -it --name test2 /root/code:/code python python /code/hello.py



vi hello.go
# go file
# go run hello.go (command to run go file)

#code is return in go file image
docker run -it --name test3 /root/code:/code go run /code/hello.go
