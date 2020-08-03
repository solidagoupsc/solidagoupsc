<?php

if(isset($_POST['submit']))
{
  $API_Key = 'AIzaSyBEHArxh-LMD4igKtsVspK2BIZnWADqJ28';
  $API_Url = 'https://www.googleapis.com/youtube/v3/';
  $channeid= $_POST['channelid'];
  $params  = array
  (
    'part' => 'snippet,contentDetails,statistics',
    'id'   => $channeid,
    'key'  => $API_Key,
  );
  $url = $API_Url.'channels?'.http_build_query($params);
  $channelDetails = json_decode(file_get_contents($url),true);
 /* print($url);
  print(file_get_contents($url));
  echo '<pre>';
 print_r($channelDetails);
  exit;*/

  $title = $channelDetails['items'][0]['snippet']['title'];
  $thumb = $channelDetails['items'][0]['snippet']['thumbnails']['medium']['url'];
  $subs = $channelDetails['items'][0]['statistics']['subscriberCount'];
  $views = $channelDetails['items'][0]['statistics']['viewCount'];
  $video = $channelDetails['items'][0]['statistics']['videoCount'];
  $params  = array
  (
    'part' => 'snippet,contentDetails',
    'playlistId'   => $channelDetails['items'][0]['contentDetails']['relatedPlaylists']['uploads'],
    'key'  => $API_Key,
    'maxResults' => 50
  );

  $url = $API_Url.'playlistItems?'.http_build_query($params);
  $playlistDetails = json_decode(file_get_contents($url),true);

  $data = $playlistDetails['items'];
}
else 
{
  $data = [];
}
?>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
 
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css">
</head>
<body>
  <section class="container py-5 text-center">
    
    <div class="row mb-5">
      <div class="col-6 mx-auto">
      
        <form action="" method="POST">
          <div class="form-group mb-4">
            <input type="text" class="form-control" placeholder="Enter channel id" name="channelid">
          </div>
          <input class="btn btn-danger" value="GET DATA" type="submit" name="submit">
        </form>
      </div>
    </div>
<table class="table table-bordered">
      <tr>
        <th>Channel Logo</th>
        <th>Channel Name</th>
        <th>Channel Subscribers</th>
        <th>Channel Views</th>
        <th>Channel Videos</th>
      </tr>
      <tr>
        <td><img src="<?php echo isset($thumb)? $thumb: ''?>" alt=""></td>
        <td><?php echo isset($title)? $title: ''?></td>
        <td><?php echo isset($subs)? $subs: ''?></td>
        <td><?php echo isset($views)? $views: ''?></td>
        <td><?php echo isset($video)? $video: ''?></td>
      </tr>
    </table>
  </section>
 <section class="container">
    <div class="row">

    <?php foreach ($data as $video) {
      $id = $video['contentDetails']['videoId'];?>
      <div class="col-3 mb-5">
        <iframe width="100%" height="200" src="https://www.youtube.com/embed/<?php echo $id?>" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
        <?php } ?>
    </div>
  </section> 
</body>
</html>
