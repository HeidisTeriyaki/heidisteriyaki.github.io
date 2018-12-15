---
title: Heidi's Teriyaki Express
position: 0
layout: default
---

	
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
			var msec = Date.parse("January 05, 2019");
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
					We will be <span class="highlightmeclosed"><b>CLOSED for Christmas & New Year </b></span> <br> from <br> <span class="cdate"> December-24-2018 </span> to <span class="cdate">January-04-2018</span> <br>
					And <br> <span class="highlightmereopen"><b>RE-OPEN</b></span><br> on Saturday <br> <span class="cdate"> January-05-2018</span> <br><br>
					<span>Thank you! Heidi's Teriyaki Express.</span>

			</div>
			<div class="modal-footer">
			  <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
			</div>
		
