desc "Build everything"
task :all => %w{ pygment:generate jekyll:run } do 
end

desc "Clean everything"
task :clean => %w{ jekyll:clean } do 
end

namespace :jekyll do
  
  desc "Run a local Jekyll server for development"
  task :server do
    system "jekyll --server --auto"
  end
  
  desc "Generate the site output in _site"
  task :run do
    system "jekyll --pygments --safe"
  end
  
  desc "Clean the generated site output in _site"
  task :clean do
    rm_rf "_site"
  end

end

namespace :pygment do
  
  desc "Generate a Pygment CSS"
  task :generate do
    system "pygmentize -f html -S colorful -a .highlight > css/syntax.css"
  end
  
end
