Starting With the name of ALLAH the most mercifull and the only creator.

Objective
-how to use clerk for simple signin signup
-role based authentication and auhtoriation with routing control


1.  for simple signin.singup just use this one pade clerkdoc and its ok done here (for nect.js app routing)
https://clerk.com/docs/quickstarts/nextjs


Hi future Sadar this is from past Sadar Hussain from date 22 APRIL 2025.
Hope so u have already became a software developer.

so get start simple ahi yar do page ak doc read kro isi se sara kaam hojayega 


2. for role based authorization
https://clerk.com/docs/references/nextjs/basic-rbac#refactor-the-admin-dashboard

isme do chise in clerk website me jakr kaam krna hoga 

2. i.      kisi user ko admin ka koi bhi role dene ke liye uske clerk me jakr us user ko like aur meta data (notes image sin the folder noteshots image 1)

**clerk->dashboard->user->select user under Metadara public add
 {role: "admin"}

2. ii. Add this in the clerk->dashboard->configure -> session ->Customize session token there will be black box add this line to it
(image in the notshot 2)
{
	"metadata": "{{user.public_metadata}}"
}

****U can leave middleware.tsx of same as given in started guide no matter  if using role or not same for both. just in role oage u can to give gice access to role  only then look for the code in the admin/page.tsx how to restrict routing for the roles ***