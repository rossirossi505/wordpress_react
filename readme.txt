//this is for react:

look at the build folder, this build folder we get for running command line on the terminal
for that look at package.json file



function boilerplate_load_assets() {
  wp_enqueue_script('ourmainjs', get_theme_file_uri('/build/index.js'), array('wp-element'), '1.0', true);
  wp_enqueue_style('ourmaincss', get_theme_file_uri('/build/index.css'));
}

add_action('wp_enqueue_scripts', 'boilerplate_load_assets');

/////////////////////

if you look carefully , react is absent in the package.json file, but still we're importing 
react, the probable cause is reat has been already imported in wordpress!!!!!!!!!!!!!!!!!!!!!!!!!!