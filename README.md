


<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head id="Head1"><meta name="robots" content="noindex" /><meta name="robots" content="nofollow" /><meta charset="utf-8" /><meta http-equiv="x-ua-compatible" content="ie=edge" /><title>
 Syntel Solutions | Phone Programming Specifications
</title><meta name="description" /><meta name="viewport" content="width=device-width, initial-scale=1" /><link rel="icon" type="image/png" href="PLACE WP LINK FOR FAVICON HERE" /><link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" rel="stylesheet" /><link href="http://getbootstrap.com/examples/jumbotron-narrow/jumbotron-narrow.css" rel="stylesheet" /><link href="css/app.css" rel="stylesheet" /></head>
<body>
    <div class="container">
        <form method="post" action="./" id="Form1">
<div class="aspNetHidden">
<input type="hidden" name="__VIEWSTATE" id="__VIEWSTATE" value="Go1FnMfxI1Vm9GQHSiONCKNaazRwiI7326v+8lsymMaA1ZZ8shIVAqcxY06z2+SMblQxfpGxEK4kJVb7/WxjU0vOLvQwoSQMAe2KJxTDfAw=" />
</div>

<div class="aspNetHidden">

 <input type="hidden" name="__VIEWSTATEGENERATOR" id="__VIEWSTATEGENERATOR" value="DCA886A8" />
 <input type="hidden" name="__EVENTVALIDATION" id="__EVENTVALIDATION" value="isqWHNULwOhuztYgd/Q6KzcWZOkCWfcKtOPqgPJ1FxRCAj0LHGjwYK3LeGxw4T+1RibcVmjd2h7oCGP0kiO2Ap3WOsK+0YpJxJ3Rk0zhw40MmCAE8iXPGoWsiLTBLb3uMpBEdk1By/Xi7JQ3VoU4Ig==" />
</div>
        <div class="row customer-form">
              <div class="header clearfix">
                <img src="URL TO LOGO ON WP GOES HERE" alt="Syntel Solutions Logo" id="logo" />
              </div>
            <h3 class="text-center">Syntel Solutions Phone Programming Specifications</h3>
            <div>
                <div class="form-group">
                    <label for="companyName">Company Name:</label>
                    <input class="form-control" type="text" id="companyName" data-bind="value: $root.companyName" placeholder="Company Name" required />
                </div>
                <div class="form-group">
                    <label for="firstName">First Name:</label>
                    <input class="form-control" type="text" id="firstName" data-bind="value: $root.firstName" placeholder="First Name" required />
                </div>                
                <div class="form-group">
                    <label for="lastName">Last Name:</label>
                    <input class="form-control" type="text" id="lastName" data-bind="value: $root.lastName" placeholder="Last Name" required />
                </div>   
                <div class="form-group">
                    <label for="email">Contact E-Mail:</label>
                    <input class="form-control" type="email" id="email" data-bind="value: $root.contactEmail" placeholder="Contact E-Mail" required />
                </div>    
                <div class="form-group">
                    <label for="phone">Contact Phone:</label>
                    <input class="form-control phoneEntry" type="tel" id="phone" data-bind="value: $root.contactPhone" placeholder="Contact Phone Number"/>
                </div>
                <div class="form-inline">
                    <label for="blinkOption">Would you like to enable International Calling?</label>                
                    <select class="form-control pull-right"  id="blinkOption" data-bind="value: blink">
                        <option value="1">Yes</option>
                        <option value="0">No</option>
                    </select>
                </div> </br>

                <div class="form-inline">
                    <label for="screenPop">Would you like 7 digit dialing?<small> (This is the ability to dial locally without the area code.) </small></label>
                    <select class="form-control pull-right"  id="screenPop" data-bind="value: screenPop">
                        <option value="1">Yes</option>
                        <option value="0">No</option>
                    </select>
   </div>
                <div class="form-group">
                    <label for="extension">If so, Please specifiy which area code:</label>
                    <input class="form-control phoneEntry" type="text" maxlength="3" id="extension" data-bind="value: $root.extension" placeholder="Area Code" required />
                </div> 
               </div>
            </div>
        </div>
        <div class="row selected-phone-options">
            <hr />
            <div class="row">
          </br>

          <html>
    <head>
        <title>Testing</title>
        <script type="text/javascript">

            function clickUpload() {
                document.getElementById("UploadFile").click();
            }

            function clickDownload() {
                document.getElementById("DownloadForm").submit();
            }

            function MakeUpload() {
                document.getElementById("UploadForm").submit();
            }

        </script>
    </head>
    <body>
            <input type="button" value="Download" onclick="clickDownload();" />
            <input type="button" value="Upload" onclick="clickUpload();" 
            <form id="UploadForm" action="test3.asp" enctype="multipart/form-data">
                <input type="file" id="UploadFile" onchange="MakeUpload();" style="display:none" />
            </form>
            <form id="DownloadForm" action="INSERT LINK TO SPREADSHEET HERE">
            </form>
    </body>
</html>
                                      <div class="col-md-4">
                                          <input type="text" class="form-control" data-bind="value: label" />
                                      </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                            <div id="">
                            <input type="submit" name="btnSendEmail" value="Send Email" onclick="CreateData();" id="btnSendEmail" class="btn btn-primary pull-right" />
                            <input type="hidden" name="dataSubmit" id="dataSubmit" />
                            <br />
                            <label hidden="hidden" data-bind="text: ko.toJSON($root)" id="hiddenData"/>
                            </div>
                    </div>
                </div>
           </div>
        </div>
        </form>
    </div>
</body>

<script src="js/jquery-2.1.4.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>
<script src="js/knockout-3.4.0.min.js"></script>
<script src="js/ViewModels/ProvisioningViewModel.js"></script>
<script src="js/jquery.alphanumeric.js"></script>
<script>
    $(document).ready(function () {

        $('.thumbnail').click(function () {

            $('#selected-name').text($(this).find('.caption').text());
            $('#selected-image').attr('src', $(this).attr('data-display-img'));
            $('#phone-properties').show();

            var startKey = parseInt($(this).attr('data-start')),
                numberKeys = parseInt($(this).attr('data-max'));

            thisViewModel.prepare(startKey, numberKeys, $(this).attr('data-phone-model'));

            thisViewModel.phoneBrand($(this).attr('data-phone-brand'));
            thisViewModel.phoneModel($(this).attr('data-phone-model'));
        });

        $('img#selected-image').load(function () {
            var pos = $('#phone-data').offset();
            $('body').animate({ scrollTop: pos.top });
        });
    });

    function CreateData() {
        document.getElementById("dataSubmit").value = document.getElementById('hiddenData').innerHTML;
    }

    $(function () {
        $('.phoneEntry').justNumeric();
    });

</script>
</html>

