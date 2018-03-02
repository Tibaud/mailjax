#MailJax

Le plus beau client mail de tout l'internet!

Pour l'app c'est par là >> https://mailjax.herokuapp.com/

Rien de fantastique, tout fonctionne.

Le seul truc funky c'est l'utilisation de la gem Faker qui permet de générer du fake contenu pour le seed:

ex: pour créer 10 objets composés d'une phrase et d'un paragraphe:

10.times do |n|
  objet  = Faker::Lorem.sentence(1)
  paraph = Faker::Lorem.paragraph(10)
  e = Email.create!(object:  objet,
              body: paraph)
end

Voilà, enjoy et bon courage pour la dernière ligne droite !

##NE LOUPE PAS MON ATELIER SEO LE 16 MARS, TU POURRA VOIR MA BOUILLE!
