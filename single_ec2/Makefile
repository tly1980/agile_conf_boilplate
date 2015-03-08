##########################################################
##                                                      ##
##  Please add following command to your ~/.bash_rc     ##
##  It allow you quickly switch between different conf  ##
##  e.g.:                                               ##
##        $> using uat agc build                        ##
##     is equivalent to:                                ##
##        $> agc build  --conf conf_uat.yaml            ##
##                                                      ##
##########################################################

BUILD_DST=$(shell agc where)
BUILD_ID=$(shell agc id)

help:
	agc shortcut

all: build after

inspect:
	agc inspect

build:
	agc build

after:
	chmod 0500 $(BUILD_DST)/*.sh

info:
	@echo "Current build id is: $(BUILD_ID)"
	@echo "Destination is: $(BUILD_DST)"