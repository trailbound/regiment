require 'rake/clean'

CLEAN
CLEAN.class

task :xmlbindings => 'ipxact.py'

file 'ipxact.py' => 'resources/schemas/IPXACT-1685-2014/index.xsd' do
  sh "pyxbgen -u ./resources/schemas/IPXACT-1685-2014/index.xsd -m ipxact"
end

CLEAN.include('ipxact.py')
