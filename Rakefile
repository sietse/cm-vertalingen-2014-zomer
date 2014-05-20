rule  '.html' => '.rst.txt' do |task|
    sh "pandoc #{task.source} --standalone > #{task.name}"
end

task :default => Dir['*.rst.txt'].map { 
    |x| x.sub(/\.rst\.txt$/, '.html') 
} do 
end
