<?php
/*********************************************************************
*
* This file is a part of Web Interface to Octave project.
* Copyright (C) 2008 Kolo Naukowe Numerykow Uniwersytetu Warszawskiego
* (Students' Numerical Scientific Group of University of Warsaw)
*
* e-mail:knn@students.mimuw.edu.pl
*
* Distributed under terms of GPL License
*
*
*********************************************************************/

require_once('code/interfaces.php');

class YourAccount implements Content
{
	private $user;
	private $allow;
	

	public function __construct($user)
	{
		$this->user = $user;
		$this->allow = !$user->IsAnonymous();
		
		
	}
	
   
    public function ShowContent()
	{
	echo '<div class="panel">';
	echo '<div>';
      
          if ($this->user->IsAnonymous())
          {
            echo '<form action="index.php?p=yc" method="post">
	    <table>
	    <tr>
	    <th><label for="login">Comment</label>
	    <td><input type="text" name="login" id="login">
	    </tr>
	  
	    </table>
            <p>         <input type="submit" value="Add Comment" >
                        </form>';  
	   
           
          }
         
	  

	}
	echo '</div>';
	} //ShowContent
}
?>
