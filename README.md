if (grep -RIZ “123” target | xargs -0 cp -t . ); then
echo “cp - OK”
else 
echo “cp - FAILS”
fi
if (grep -RLZ “123” target | xargs -0 rm); then
	echo “rm - OK” 
else 
echo “rm - FAILS”\
fi
