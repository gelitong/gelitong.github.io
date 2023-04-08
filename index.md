Space shoot
==========================
Space shoot is about a shooting game.
![12345678](https://user-images.githubusercontent.com/119718674/230703423-f8970e1a-d6a2-46dc-830d-91c5bffe0750.png)

![Screenshot 2023-04-08 124125](https://user-images.githubusercontent.com/119718674/230703472-9ce4c59b-afab-4f6b-ae02-4868bd1260a4.png)

Method
=========

  - You can press A and D to move.
  - If you press "space" and you can just kill the "Enemy"
    and you will get points!
    
  
Features
=============== 
- The game have very special planets to shoot.
- You are the alian to shoot those planets!
- The stars background!
- The  interesting code of plants
   
   ~~~pyson 
   class Enemy(Sprite):
    def on_create(self):
        self.image=get_random_file_from_directory('Planets/')
        self.scale=0.09
        self.goto_random_position() 
        self.x=1000
        self.add_tag("Enemy")
    def on_update(self, dt):
        self.x-=5       
        if self.is_touching_window_edge():
            self.delete()
        if self.is_touching_any_sprite_with_tag("Bullet"):
            self.delete()
                     

Resources
=============
- pycat/pyson
- [Tiny Ski-kenney](https://www.kenney.nl/assets/tiny-ski)






