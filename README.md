# Compose Everything

This is aimed for complete beginners in Flutter, to get them acquainted with the various basic widgets in Flutter. 
 
# Examples

### ImageView

<table>
 <tr><td> <b>Simple Image</b> </td></tr>
 
 <td>
  <pre> 
  val avatarImage =  imageResource(R.drawable.avatar)
  Image(avatarImage)
        
   </pre>
</td>
 
  <tr><td> <b>Circular Image</b> </td></tr>
  <tr>
<td>
  <pre> 
  val avatarImage =  imageResource(R.drawable.avatar)
  val imageModifier = Modifier
                     .preferredHeight(100.dp)
                     .preferredWidth(100.dp)
                     .fillMaxWidth()
                     .clip(shape = RoundedCornerShape(50.dp))
            
            
   <br>
  Image(avatarImage,  modifier = imageModifier,contentScale = ContentScale.Crop)
        
   </pre>
</td>

</tr>
  </table>
  
  
### Button

<table>
 <tr><td> <b>Icon Button</b> </td></tr>
 <tr>
 <td>
  <pre> 
  IconButton(onClick = {
                //
                }, icon = {
                    Icon(asset = Icons.Default.Close)
                   }
  )
   </pre>
</td>
</tr>
</table>

### Others

<table>
 <tr>
  <td> <b>Divider</b> </td>
   <td> <b>Spacer</b> </td>
 </tr>
 <tr>
 <td>
  <pre> 
  Divider(
       thickness = 1.dp,
       color = colGray
   )
   </pre>
</td>
  
  <td>
  <pre> 
  Spacer(modifier = 
       Modifier.preferredHeight(40.dp)
  )
   </pre>
</td>
  
</tr>
</table>

