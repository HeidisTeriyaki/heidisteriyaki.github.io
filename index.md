---
title: Heidi's Teriyaki Express
position: 0
layout: default
---

![Heidi's Teriyaki Express Storefront](/uploads/storefront.jpg)

<p><b>Phone Number:</b> <br/><a href="360-662-0060">(360) 662-0060</a><br/></p>

<p><b>Hours:</b><br/>

MON - SAT: 11:00 AM - 8:00 PM<br/>  
SUN: CLOSED<br/> 
(Dine-In Closed @ 7:50PM--Take-Out ONLY)<br/>
<p/>
 
<p><b>Address:</b><br/>
3014 NW Bucklin Hill Road<br/>
Silverdale, WA 98383<br/>
(Across from Staples and Jo-Ann)<br/>
</p>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2687.707223349842!2d-122.69196668436793!3d47.65125597918769!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54903a9432099a4b%3A0x88500a0880d8fef4!2sHeidi\+Teriyaki\+Express!5e0!3m2!1sen!2sus!4v1469594514828" height="450" width="100%" frameborder="0" style="border:0" allowfullscreen></iframe> 
 
		<style>
		.notice {text-align: center;}
		.highlightme { background-color:#FFFF00; font-size: 150%; }
		.highlightmeclosed { background-color:#ff9966; font-size: 150%; }
		.highlightmereopen { background-color:#66ccff; font-size: 150%; }
		
		.cdate { background-color:#FFFF00; font-size: 150%; }
	</style>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
	<div id="temp">
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
	</div>
	
	<script>
		$( document ).ready(function(){
			var timeInMs = Date.now();			
			var msec = Date.parse("December 28, 2021");
			if(timeInMs < msec)
				$("#btn_modal").click();
			else
			{
				if($("#temp").length > 0)
					$("#temp").remove();
			}
			
			$('#myModal').on('hidden.bs.modal', function () {
				// do something…
				if($("#temp").length > 0)
					$("#temp").remove();
			})			
			
		});
	</script>	
	
	<div class="container">	
	  <!-- Trigger the modal with a button -->
	  <button type="hidden" style="display:none" id="btn_modal" class="btn btn-info btn-lg" data-toggle="modal" data-target="#myModal"></button>

	  <!-- Modal -->
	  <div class="modal fade" id="myModal" role="dialog">
		<div class="modal-dialog">
		
		  <!-- Modal content-->
		  <div class="modal-content notic">
			<div class="modal-header">
			  <button type="button" class="close" data-dismiss="modal">&times;</button>
			  <h4 class="modal-title">NOTIFICATION </h4>
			</div>
			<div class="modal-body">
			  <p style="word-wrap: break-word;">
				<div class="notice">
					We will be <span class="highlightmeclosed"><b>CLOSED for New Year Holiday </b></span><br> on Friday <br>  <span class="cdate"> January-01-2021 </span>  <br>
					And <br> <span class="highlightmereopen"><b>RE-OPEN</b></span><br> on Saturday <br> <span class="cdate"> January-02-2021</span> <br><br>
					<h4>Note: Currently, our restaurant take orders for</h4> <span class="cdate"> CARRY-OUT ONLY </span><br><br>
					<span>Thank you! Heidi's Teriyaki.</span>

			</div> 
			<div class="modal-footer">
			  <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
			</div>
		 