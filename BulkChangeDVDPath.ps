############################################################################################
# Name	: BulkChangeDVDPath.ps                                                             #
# Author: Andrew Cracknell                                                                 #
# Date	: 23/06/2017                                                                       #
# Why	: Shared Storage Location for VM ISOs changed so needed to bulk modify Templates   #
############################################################################################
# Version History                                                                          #
# ----------------                                                                         #
# Who	Description                                                                        #
# AC	Initial script built                                                               #
# AC    Made script more generic                                                           #
############################################################################################

# Get the VM's DVD Drives where there's an ISO attachment and loop through the results
Get-VMDvdDrive * | ? DvdMediaType -eq ISO | ForEach-Object {

	# Search the DVD path for a pattern of the old network path
	if ( $_.Path -match "Persistent_ISOs" ) {

		# Build a new path by replacing one string for another
		$newpath = $_.Path -replace "Persistent_ISOs", "ISOs"

		# DEBUG option: Print to screen the old and new path
		write-host "Old Path: $_.Path | New Path: $newpath"

		# Update each VM's specific DVD path to the new path
		Set-VMDvdDrive -VMName $_.VMName -ControllerNumber $_.ControllerNumber -ControllerLocation $_.ControllerLocation -Path $newpath

	}		
}