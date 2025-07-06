Tento repozitář byl vytvořen za účelem splnění úkolu k pracovní nabídce.

Default user v playbooks/hosts.ini je uživatel "admin", pokud jste momentálně lognuti jako uživatel s jiným jménem, ansible playbook nepůjde spustit.

Postup:
1. sudo apt install openssh-server
2. sudo apt install ansible
3. Vytvořte si ssh  klíč k naklonování repozitáře.
4. Naklonovat tento repozitář, nejlépe do složky /home/$(jméno uživatele)/
5. Spusťte playbook skrze: ansible-playbook -i inventory/hosts.ini playbooks/site.yml
