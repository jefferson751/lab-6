# Atualizar os pacotes e instale o Apache2

# comandos:
sudo apt-get update sudo
apt-get install apache2

# Criar uma página de teste simples

# Comandos:
echo "<h1>Bem-vindo ao Servidor Web da Empresa!</h1>" 
sudo tee /var/www/html/index.html

# instalar o bind9

# Comando:
sudo apt-get install bind9

# Configuar uma nova zona no BIND

# comandos: 
sudo nano /etc/bind/named.conf.local

# Reiniciar o serviço BIND:
# Comandos:
sudo systemctl restart bind9

# Configurar o DNS da VM
# Comandos:
/etc/resolv.conf:

# Adicionar no em cima:
# Comandos:
nameserver 127.0.0.1
sudo nano /etc/bind/named.conf.local
