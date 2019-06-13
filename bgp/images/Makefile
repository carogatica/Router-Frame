all:
	sudo docker-compose up -d
	sudo docker exec -ti images_h1_1 route del default;
	sudo docker exec -ti images_DNSFrame_1 route del default;
	sudo docker exec -ti images_h1_1 route add default gw 200.9.20.3;
	sudo docker exec -ti images_DNSFrame_1 route add default gw 200.9.21.34;
    sudo docker exec -ti images_b1_1 route del default;
    sudo docker exec -ti images_b1_1 route add default gw 70.0.0.6; 
d_clean:
	sudo docker-compose down