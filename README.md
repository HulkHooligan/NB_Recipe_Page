# NB_Recipe_Page
Recipe page for Omron NB HMIs
was created on 29/5/2022 for educational purposes only

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.

The page is configured for an NB10W connected via ethernet to an NX1 series PLC
with a limit of 100 recipes. There are 3 settings for each recipe which can be
expanded/shortened, with the exception of words RW1000 - RW1100. There is a 
10 word description (20 characters) which is saved in the HMI. The working recipe
is at the top of the list, it can be selected by inputing the recipe number or
by using the up and down arrows. The 'Send to PLC' button sends the 3 settings
of the working recipe to the PLC at addresses D400 (setting 1), D402 (setting 2)
and D404 (setting 3). The page runs a small macro in the background which creates
a seperate index for the description text memory.

The password to decompile the .pkg file is: 888888
