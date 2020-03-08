sh_path=$(cd "$(dirname "${BASH_SOURCE-$0}")"; pwd)
cd ${sh_path}

for file in `ls ${sh_path}`;
do mv $file `
echo $file|sed 's/.png/@3x.png/g'`