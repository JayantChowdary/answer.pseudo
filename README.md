# answer.pseudo
Jobspire Challenge 

JOBSPIRE_CHALLENGE CONTROLLER:

<?php 
session_start();
  class Jobspire_challenge extends CI_Controller
  {
      function __construct()
	  	{
		    parent::__construct();
	  	}
	  	
	  	function GetChar($name)
	  	{
	  	  $data['string']=$name;
	  	  $data['RandomNumber']=rand(6,15);
	  	  $this->load->view('jobspire_challenge_view',$string,$RandomNumber);
	  	}
  }
?>

JOBSPIRE_CHALLENGE_VIEW    VIEW:

<?php 

echo "$string"."$RandomNumber";

?>
