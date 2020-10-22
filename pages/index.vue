<template>

<div class="section">
   <div id="ao3SearchForm" class="container">

       <form action="https://mrdholidays.golibe.com/index.php" method="post" class="ui-front">
        <div>
          <input type="hidden" name="data[lastStep]" value="OneMultiple" />
          <input type="hidden" name="lang" value="1" />
          <input type="hidden" name="action" value="eSearchFormStaticData" />
          <input type="hidden" value="" name="data[AO3SOReference]" />
          <input type="hidden" value="" class="j-departurePlusMinusDay" name="data[flights][0][departurePlusMinusDay]" />
          <input type="hidden" value="" class="j-departurePlusMinusDay" name="data[flights][1][departurePlusMinusDay]" />      
          
          <div class="z-depth-1 layer1">
            <div class="cleared">
              <div class="left j-returnTicketModeDiv">
                <input type="radio" name="data[returnTicket]" id="AO3_StepOne2_returnTicketNo" value="" class="hidden j-returnTicketMode" />
                <label for="AO3_StepOne2_returnTicketNo" class="cursorClickable btn-icon icon-oneway" title="One-way"></label>
              </div>
              <div class="left j-returnTicketModeDiv">
                <input type="radio" name="data[returnTicket]" id="AO3_StepOne2_returnTicketYes" value="on" class="hidden j-returnTicketMode" checked="checked" />
                <label for="AO3_StepOne2_returnTicketYes" class="cursorClickable btn-icon icon-return" title="Return"></label>
              </div>
              <div class="left j-returnTicketModeDiv j-multipleDestination">
                <input type="radio" name="data[returnTicket]" id="AO3_StepOne2_returnTicketMulti" value="multi" class="hidden j-returnTicketMode" />
                <label for="AO3_StepOne2_returnTicketMulti" class="cursorClickable btn-icon icon-multi" title="Multiple"></label>
              </div>
              <div class="left j-returnTicketModeDiv j-redirectToHotels hidden">
                <a class="cursorClickable btn-icon icon-hotel" title="Hotels" href="https://mrdholidays.golibe.com/index.php?action=vHotels" style="text-decoration: none; color:inherit;"></a>
              </div>
            </div>
            <div class="col">
              <input type="hidden" name="data[selectionCounter]" value="" />
              <div class="row j-flightSegment" data-segment-index="0">
                <div class="col s12 l4">
                  <input type="text" autocomplete="off" name="data[flights][0][originSearch]" id="AO3_StepOne2_origin_0" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="0" placeholder="Origin" />
                  <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="0"></span>
                  <input type="hidden" id="exact_origin_0" class="j-flightOriginCode" data-segment-index="0" name="data[flights][0][origin]" />
                  <input type="button" name="data[stepChooseOrigin][seg_0]" id="AO3_StepOne2_originButton_0" value="Choose" class="hidden" />
                </div>

                
                <div class="col s12 l4">
                  <input type="text" autocomplete="off" name="data[flights][0][destinationSearch]" id="AO3_StepOne2_destination_0" value="" class="j-enableGoogleMapsLink j-flightDestination" data-segment-index="0" placeholder="Destination" />
                  <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="0"></span>
                  <input type="hidden" id="exact_destination_0" class="j-flightDestinationCode" data-segment-index="0" name="data[flights][0][destination]" />
                  <input type="button" name="data[stepChooseDestination][seg_0]" id="AO3_StepOne2_destinationButton_0" value="Choose" class="hidden" />
                </div>
                <div class="j-returnMultiView">
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="0">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][0][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="0" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="0">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="0">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="0" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="col s12 l4 j-returnYesView j-returnNoView">
                  <input type="text" autocomplete="off" readonly="readonly" class="j-passengersSummary inputWithIconInside" placeholder="Passengers & class" />
                  <span class="icon-arrowDown iconInsideInput cursorClickable j-passengersDetailOpen"></span>
                </div>
              </div>
              <div class="j-returnMultiView">
                <div class="row j-flightSegment" data-segment-index="1">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][1][originSearch]" id="AO3_StepOne2_origin_1" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="1" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="1"></span>
                    <input type="hidden" id="exact_origin_1" class="j-flightOriginCode" data-segment-index="1" name="data[flights][1][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_1]" id="AO3_StepOne2_originButton_1" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][1][destinationSearch]" id="AO3_StepOne2_destination_1" data-segment-index="1" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="1"></span>
                    <input type="hidden" id="exact_destination_1" class="j-flightDestinationCode" data-segment-index="1" name="data[flights][1][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_1]" id="AO3_StepOne2_destinationButton_1" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="1">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][1][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="1" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="1">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="1">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="1" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="2">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][2][originSearch]" id="AO3_StepOne2_origin_2" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="2" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="2"></span>
                    <input type="hidden" id="exact_origin_2" class="j-flightOriginCode" data-segment-index="2" name="data[flights][2][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_2]" id="AO3_StepOne2_originButton_2" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][2][destinationSearch]" id="AO3_StepOne2_destination_2" data-segment-index="2" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="2"></span>
                    <input type="hidden" id="exact_destination_2" class="j-flightDestinationCode" data-segment-index="2" name="data[flights][2][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_2]" id="AO3_StepOne2_destinationButton_2" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="2">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][2][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="2" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="2">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="2">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="2" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="3">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][3][originSearch]" id="AO3_StepOne2_origin_3" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="3" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="3"></span>
                    <input type="hidden" id="exact_origin_3" class="j-flightOriginCode" data-segment-index="3" name="data[flights][3][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_3]" id="AO3_StepOne2_originButton_3" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][3][destinationSearch]" id="AO3_StepOne2_destination_3" data-segment-index="3" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="3"></span>
                    <input type="hidden" id="exact_destination_3" class="j-flightDestinationCode" data-segment-index="3" name="data[flights][3][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_3]" id="AO3_StepOne2_destinationButton_3" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="3">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][3][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="3" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="3">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="3">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="3" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="4">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][4][originSearch]" id="AO3_StepOne2_origin_4" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="4" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="4"></span>
                    <input type="hidden" id="exact_origin_4" class="j-flightOriginCode" data-segment-index="4" name="data[flights][4][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_4]" id="AO3_StepOne2_originButton_4" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][4][destinationSearch]" id="AO3_StepOne2_destination_4" data-segment-index="4" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="4"></span>
                    <input type="hidden" id="exact_destination_4" class="j-flightDestinationCode" data-segment-index="4" name="data[flights][4][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_4]" id="AO3_StepOne2_destinationButton_4" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="4">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][4][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="4" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="4">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="4">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="4" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="5">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][5][originSearch]" id="AO3_StepOne2_origin_5" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="5" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="5"></span>
                    <input type="hidden" id="exact_origin_5" class="j-flightOriginCode" data-segment-index="5" name="data[flights][5][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_5]" id="AO3_StepOne2_originButton_5" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][5][destinationSearch]" id="AO3_StepOne2_destination_5" data-segment-index="5" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="5"></span>
                    <input type="hidden" id="exact_destination_5" class="j-flightDestinationCode" data-segment-index="5" name="data[flights][5][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_5]" id="AO3_StepOne2_destinationButton_5" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="5">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][5][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="5" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="5">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="5">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="5" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="6">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][6][originSearch]" id="AO3_StepOne2_origin_6" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="6" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="6"></span>
                    <input type="hidden" id="exact_origin_6" class="j-flightOriginCode" data-segment-index="6" name="data[flights][6][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_6]" id="AO3_StepOne2_originButton_6" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][6][destinationSearch]" id="AO3_StepOne2_destination_6" data-segment-index="6" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="6"></span>
                    <input type="hidden" id="exact_destination_6" class="j-flightDestinationCode" data-segment-index="6" name="data[flights][6][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_6]" id="AO3_StepOne2_destinationButton_6" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="6">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][6][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="6" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="6">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="6">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="6" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
                <div class="row j-flightSegment j-flightSegmentHidden" data-segment-index="7">
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][7][originSearch]" id="AO3_StepOne2_origin_7" value="" class="j-enableGoogleMapsLink j-flightOrigin" data-segment-index="7" placeholder="Origin" />
                    <span class="icon-arrowDown iconInsideInput j-chooseOriginButton cursorClickable" data-segment-index="7"></span>
                    <input type="hidden" id="exact_origin_7" class="j-flightOriginCode" data-segment-index="7" name="data[flights][7][origin]" />
                    <input type="button" name="data[stepChooseOrigin][seg_7]" id="AO3_StepOne2_originButton_7" value="Choose" class="hidden" />
                  </div>
                  <div class="col s12 l4">
                    <input type="text" autocomplete="off" name="data[flights][7][destinationSearch]" id="AO3_StepOne2_destination_7" data-segment-index="7" value="" class="j-enableGoogleMapsLink j-flightDestination" placeholder="Destination" />
                    <span class="icon-arrowDown iconInsideInput j-chooseDestinationButton cursorClickable" data-segment-index="7"></span>
                    <input type="hidden" id="exact_destination_7" class="j-flightDestinationCode" data-segment-index="7" name="data[flights][7][destination]" />
                    <input type="button" name="data[stepChooseDestination][seg_7]" id="AO3_StepOne2_destinationButton_7" value="Choose" class="hidden" />
                  </div>
                  <div class="col l3 s10">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="7">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][7][departureDateInput]" value="" class="inputText date j-returnMultiEnabled j-departureDate" data-segment-index="7" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="7">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="7">&gt;</span>
                  </div>
                  <div class="col l1 s2">
                    <span class="icon-gol-flights cursorClickable j-hideFlightSegment colorRemove iconInsideInput" data-segment-index="7" title="- Remove this part of the journey">X</span>
                  </div>
                </div>
              </div>
              <div class="row">
                <div class="j-returnYesView j-returnNoView">
                  <div class="col l4 s12">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="0">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][0][departureDateInput]" value="" class="inputText date j-returnYesEnabled j-returnNoEnabled j-departureDate" data-segment-index="0" title="Departure" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="0">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="0">&gt;</span>
                  </div>
                </div>
                <div class="j-returnYesView">
                  <div class="col l4 s12 j-DateVariantWeekendHidden">
                    <span class="j-departureDateDay iconInsideInputLeft" data-segment-index="1">&nbsp;</span>
                    <input type="text" autocomplete="off" name="data[flights][1][departureDateInput]" value="" class="inputText date j-returnYesEnabled j-departureDate" data-segment-index="1" title="Return" />
                    <span class="icon-gol-flights cursorClickable j-departureDateDayMinus iconInsideInput2th" data-segment-index="1">&lt;</span>
                    <span class="icon-gol-flights cursorClickable j-departureDateDayPlus iconInsideInput" data-segment-index="1">&gt;</span>
                  </div>
                </div>
              </div>
              <div class="row j-returnMultiView">
                <div class="col s10 l4">
                  <input type="text" autocomplete="off" readonly="readonly" class="j-passengersSummary inputWithIconInside" placeholder="Passengers & class" />
                  <span class="icon-arrowDown iconInsideInput cursorClickable j-passengersDetailOpen"></span>
                </div>
                <div class="col s2 l8">
                  <span class="icon-gol-flights cursorClickable j-addFlightSegment iconInsideInput" title="+ Add flight">+</span>
                </div>
              </div>
            </div>
          </div>
          <div class="grey lighten-3 z-depth-1 layer2">
            <div class="row">
              <div class="col l10 topGap">
                <div class="row">
                  <div class="col l3 s12 j-flexiOnly">
                    <select name="data[dateVariants]" class="d-selectmenu j-dateVariants j-returnYesEnabled j-fromFourOnly">
                      <option disabled="disabled">Date variants</option>
                      <option value="exact" selected="selected">Exact dates</option>
                      <option value="close" data-departurePlusMinusDay="1">+/- 1 day</option>
                      <option value="close" data-departurePlusMinusDay="2">+/- 2 days</option>
                      <option value="close" data-departurePlusMinusDay="3">+/- 3 days</option>
                      <option value="weekend">Prolonged weekends</option>
                    </select>
                  </div>
                  <div class="col l3 s12">
                    <select name="data[vendor]" class="d-selectmenu j-vendor">
                      <option disabled="disabled">Airline</option>
                    </select>
                  </div>
                  <div class="col l3 s12">
                    <select name="data[searchType]" class="d-selectmenu j-searchType j-returnNoEnabled j-returnYesEnabled">
                      <option disabled="disabled">Search type</option>
                      <option value="Avail">Based on Schedule</option>
                      <option value="FromFour" selected="selected">Based on total price</option>
                    </select>
                  </div>
                  <div class="col l3 s12">
                    <select name="data[directFlight]" id="AO3_StepOne2_directFlight" class="d-selectmenu">
                      <option value="">Including transfers</option>
                      <option value="1">Only direct flights</option>
                    </select>
                  </div>
                </div>
              </div>
              <div class="col l2 s12">
                <input type="submit" name="data[stepSearchTypeRedirect]" value="Continue" class="cursorClickable activeBackground" />
              </div>
            </div>
            <div class="clear">
              <script src="https://www.google.com/recaptcha/api.js?onload=captchaOnloadCallback&render=explicit&hl=1" async defer></script>
              <div id="j-captcha"></div>
            </div>
          </div>
        </div>
        <div class="j-chooseDestination hidden ui-front">
          <div class="row">
            <div class="col l12 s12">
              <select class="d-selectmenu j-chooseCountry">
              </select>
              <select class="d-selectmenu j-chooseSubCountry">
              </select>
              <select class="d-selectmenu j-choosePlace">
              </select>
            </div>
          </div>
        </div>
        <div class="j-passengersDetail hidden ui-front">
          <div id="AO3_StepOne2_cabin" class="row">
            <div class="col l12 s12">
              <label for="AO3_StepOne2_cabin">Class:</label>
              <select name="data[cabin]" class="d-selectmenu j-fromFourOnly j-cabinClass">
                 <option value="" selected="selected">Economy</option>
                 <option value="PremiumEconomy">Premium Economy</option>
                 <option value="Business">Business</option>
              </select>
            </div>
          </div>
          <div class="row">
            <div id="AO3_StepOne2_travelersTypeCount">
              <div class="col l2 s6">
                <label for="AO3_StepOne2_travelersCountADT">Adult &nbsp;</label>
                <select name="data[travelersCount][ADT]" id="AO3_StepOne2_travelersCountADT" class="d-selectmenu j-travelersCount j-travelerCompany">
                  <option value="0">0</option>
                  <option value="1" selected="selected">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  <option value="5">5</option>
                  <option value="6">6</option>
                  <option value="7">7</option>
                  <option value="8">8</option>
                  <option value="9">9</option>
                </select>
              </div>
              <div class="col l2 s6">
                <label for="AO3_StepOne2_travelersCountINF">Infant (up to 2 years)</label>
                <select name="data[travelersCount][INF]" id="AO3_StepOne2_travelersCountINF" class="d-selectmenu j-travelersCount  j-infantNeedCompany">
                  <option value="0" selected="selected">0</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  <option value="5">5</option>
                  <option value="6">6</option>
                  <option value="7">7</option>
                  <option value="8">8</option>
                  <option value="9">9</option>
                </select>
              </div>
              <div class="col l2 s6">
                <label for="AO3_StepOne2_travelersCountCHD">Child (2-11)</label>
                <select name="data[travelersCount][CHD]" id="AO3_StepOne2_travelersCountCHD" class="d-selectmenu j-travelersCount j-childNeedCompany">
                  <option value="0" selected="selected">0</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  <option value="5">5</option>
                  <option value="6">6</option>
                  <option value="7">7</option>
                  <option value="8">8</option>
                  <option value="9">9</option>
                </select>
              </div>
              <div class="col l2 s6">
                <label for="AO3_StepOne2_travelersCountYTH">Youth (12-24)</label>
                <select name="data[travelersCount][YTH]" id="AO3_StepOne2_travelersCountYTH" class="d-selectmenu j-travelersCount j-travelerCompany">
                  <option value="0" selected="selected">0</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  <option value="5">5</option>
                  <option value="6">6</option>
                  <option value="7">7</option>
                  <option value="8">8</option>
                  <option value="9">9</option>
                </select>
              </div>
              <div class="col l2 s6">
                <label for="AO3_StepOne2_travelersCountYCD">Senior (60 and more)</label>
                <select name="data[travelersCount][YCD]" id="AO3_StepOne2_travelersCountYCD" class="d-selectmenu j-travelersCount j-travelerCompany">
                  <option value="0" selected="selected">0</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  <option value="5">5</option>
                  <option value="6">6</option>
                  <option value="7">7</option>
                  <option value="8">8</option>
                  <option value="9">9</option>
                </select>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col l12 s12">
              <div class="j-errorInfantsWithoutCompany colorError hidden">
                Infants cannot travel without company.
              </div>
              <div class="j-errorChildsWithoutCompany colorError hidden">
                Children cannot travel alone.
              </div>
              <div class="j-errorTooManyTravelerTypes colorError hidden">
                Maximum count of traveller types is 4.
              </div>
              <div class="j-errorNoTravelerSelected colorError hidden">
                You have to choose at least one traveller.
              </div>
              <div class="j-errorTooManyTravelers colorError hidden">
                Maximum count of travellers is 9.
              </div>
            </div>
          </div>
        </div>
      </form>
    </div>
</div>




</template>

<script>

export default {
head:{
  title:'flight',
  meta: [
    {charset:"utf-8"},
    {name:"viewport"}
  ],

  link: [
      { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }
    ],

script: [
  {
    src: 'components/config.1.js',
    type:'text/javascript'
  },
  {
    src: 'components/flight-d4.js',
    type:'text/javascript'
   },
   {
     src:'//jqueryui.com/jquery-wp-content/themes/jquery/js/modernizr.custom.2.8.3.min.js'
   },
    {
     src:'https://code.jquery.com/jquery-1.11.3.js'
   },
   {
     src:'//jqueryui.com/jquery-wp-content/themes/jquery/js/plugins.js'
   },
   {
     src:'//jqueryui.com/jquery-wp-content/themes/jquery/js/main.js'
   },
   {
     src:'https://use.typekit.net/wde1aof.js'
   }
   
],


}
}
</script>

<style scoped>
.section{
  background-color: yellowgreen;
}

@font-face {
  font-family: 'gol-flights';
  src:  url('../assets/images/fonts/gol-flights.eot?c5d9fe3');
  src:  url('../assets/images/fonts/gol-flights.eot?c5d9fe3#iefix') format('embedded-opentype'),
    url('../assets/images/fonts/gol-flights.ttf?c5d9fe3') format('truetype'),
    url('../assets/images/fonts/gol-flights.woff?c5d9fe3') format('woff'),
    url('../assets/images/fonts/gol-flights.svg?c5d9fe3#gol-flights') format('svg');
  font-weight: normal;
  font-style: normal;
}

.ui-front{
  background-color: black;
}

.icon-return, .icon-remove, .icon-oneway, .icon-multi, .icon-arrowDown, .icon-add, .icon-arrowLeft, .icon-arrowRight, .icon-share, .icon-hotel, .icon-gol-flights {
  /* use !important to prevent issues with browser extensions that change fonts */
  font-family: 'gol-flights' !important;
  speak: none;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1em;

  /* Better Font Rendering =========== */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.icon-return:before {
  content: "R";
}
.icon-remove:before {
  content: "X";
}
.icon-oneway:before {
  content: "O";
}
.icon-multi:before {
  content: "M";
}
.icon-arrowDown:before {
  content: "V";
}
.icon-add:before {
  content: "+";
}
.icon-arrowLeft:before {
  content: "<";
}
.icon-arrowRight:before {
  content: ">";
}
.icon-share:before {
  content: "S";
}
.icon-hotel:before {
  content: "h";
}

/*!
 * jQuery UI CSS Framework 1.11.4
 * http://jqueryui.com
 *
 * Copyright jQuery Foundation and other contributors
 * Released under the MIT license.
 * http://jquery.org/license
 *
 * http://api.jqueryui.com/category/theming/
 */

/* Layout helpers
----------------------------------*/
.ui-helper-hidden,
#ao3SearchForm .ui-helper-hidden {
	display: none;
}
.ui-helper-hidden-accessible,
#ao3SearchForm .ui-helper-hidden-accessible {
	border: 0;
	clip: rect(0 0 0 0);
	height: 1px;
	margin: -1px;
	overflow: hidden;
	padding: 0;
	position: absolute;
	width: 1px;
}
#ao3SearchForm .ui-helper-reset {
	margin: 0;
	padding: 0;
	border: 0;
	outline: 0;
	line-height: 1.3;
	text-decoration: none;
	font-size: 100%;
	list-style: none;
}
#ao3SearchForm .ui-helper-clearfix:before,
#ao3SearchForm .ui-helper-clearfix:after {
	content: "";
	display: table;
	border-collapse: collapse;
}
#ao3SearchForm .ui-helper-clearfix:after {
	clear: both;
}
#ao3SearchForm .ui-helper-clearfix {
	min-height: 0; /* support: IE7 */
}
#ao3SearchForm .ui-helper-zfix {
	width: 100%;
	height: 100%;
	top: 0;
	left: 0;
	position: absolute;
	opacity: 0;
	filter:Alpha(Opacity=0); /* support: IE8 */
}

#ao3SearchForm .ui-front {
	z-index: 100;
}


/* Interaction Cues
----------------------------------*/
#ao3SearchForm .ui-state-disabled {
	cursor: default !important;
}


/* Icons
----------------------------------*/

/* states and images */
#ao3SearchForm .ui-icon {
	display: block;
	text-indent: -99999px;
	overflow: hidden;
	background-repeat: no-repeat;
}


/* Misc visuals
----------------------------------*/

/* Overlays */
#ao3SearchForm .ui-widget-overlay {
	position: fixed;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
}
/*!
 * jQuery UI CSS Framework 1.11.4
 * http://jqueryui.com
 *
 * Copyright jQuery Foundation and other contributors
 * Released under the MIT license.
 * http://jquery.org/license
 *
 * http://api.jqueryui.com/category/theming/
 *
 * To view and modify this theme, visit http://jqueryui.com/themeroller/
 */


/* Component containers
----------------------------------*/
#ao3SearchForm .ui-widget {
	font-family: Verdana,Arial,sans-serif/*{ffDefault}*/;
	font-size: 1.1em/*{fsDefault}*/;
}
#ao3SearchForm .ui-widget .ui-widget {
	font-size: 1em;
}
#ao3SearchForm .ui-widget input,
#ao3SearchForm .ui-widget select,
#ao3SearchForm .ui-widget textarea,
#ao3SearchForm .ui-widget button {
	font-family: Verdana,Arial,sans-serif/*{ffDefault}*/;
	font-size: 1em;
}
#ao3SearchForm .ui-widget-content {
	border: 1px solid #aaaaaa/*{borderColorContent}*/;
	background: #ffffff/*{bgColorContent}*/ url("../assets/images/ui-bg_flat_75_ffffff_40x100.png")/*{bgImgUrlContent}*/ 50%/*{bgContentXPos}*/ 50%/*{bgContentYPos}*/ repeat-x/*{bgContentRepeat}*/;
	color: #222222/*{fcContent}*/;
}
#ao3SearchForm .ui-widget-content a {
	color: #222222/*{fcContent}*/;
}
#ao3SearchForm .ui-widget-header {
	border: 1px solid #aaaaaa/*{borderColorHeader}*/;
	background: #cccccc/*{bgColorHeader}*/ url("../assets/images/ui-bg_highlight-soft_75_cccccc_1x100.png")/*{bgImgUrlHeader}*/ 50%/*{bgHeaderXPos}*/ 50%/*{bgHeaderYPos}*/ repeat-x/*{bgHeaderRepeat}*/;
	color: #222222/*{fcHeader}*/;
	font-weight: bold;
}
#ao3SearchForm .ui-widget-header a {
	color: #222222/*{fcHeader}*/;
}

/* Interaction states
----------------------------------*/
#ao3SearchForm .ui-state-default,
#ao3SearchForm .ui-widget-content .ui-state-default,
#ao3SearchForm .ui-widget-header .ui-state-default {
	border: 1px solid #d3d3d3/*{borderColorDefault}*/;
	background: #e6e6e6/*{bgColorDefault}*/ url("../assets/images/ui-bg_glass_75_e6e6e6_1x400.png")/*{bgImgUrlDefault}*/ 50%/*{bgDefaultXPos}*/ 50%/*{bgDefaultYPos}*/ repeat-x/*{bgDefaultRepeat}*/;
	font-weight: normal/*{fwDefault}*/;
	color: #555555/*{fcDefault}*/;
}
#ao3SearchForm .ui-state-default a,
#ao3SearchForm .ui-state-default a:link,
#ao3SearchForm .ui-state-default a:visited {
	color: #555555/*{fcDefault}*/;
	text-decoration: none;
}
#ao3SearchForm .ui-state-hover,
#ao3SearchForm .ui-widget-content .ui-state-hover,
#ao3SearchForm .ui-widget-header .ui-state-hover,
#ao3SearchForm .ui-state-focus,
#ao3SearchForm .ui-widget-content .ui-state-focus,
#ao3SearchForm .ui-widget-header .ui-state-focus {
	border: 1px solid #999999/*{borderColorHover}*/;
	background: #dadada/*{bgColorHover}*/ url("../assets/images/ui-bg_glass_75_dadada_1x400.png")/*{bgImgUrlHover}*/ 50%/*{bgHoverXPos}*/ 50%/*{bgHoverYPos}*/ repeat-x/*{bgHoverRepeat}*/;
	font-weight: normal/*{fwDefault}*/;
	color: #212121/*{fcHover}*/;
}
#ao3SearchForm .ui-state-hover a,
#ao3SearchForm .ui-state-hover a:hover,
#ao3SearchForm .ui-state-hover a:link,
#ao3SearchForm .ui-state-hover a:visited,
#ao3SearchForm .ui-state-focus a,
#ao3SearchForm .ui-state-focus a:hover,
#ao3SearchForm .ui-state-focus a:link,
#ao3SearchForm .ui-state-focus a:visited {
	color: #212121/*{fcHover}*/;
	text-decoration: none;
}
#ao3SearchForm .ui-state-active,
#ao3SearchForm .ui-widget-content .ui-state-active,
#ao3SearchForm .ui-widget-header .ui-state-active {
	border: 1px solid #aaaaaa/*{borderColorActive}*/;
	background: #ffffff/*{bgColorActive}*/ url("../assets/images/ui-bg_glass_65_ffffff_1x400.png")/*{bgImgUrlActive}*/ 50%/*{bgActiveXPos}*/ 50%/*{bgActiveYPos}*/ repeat-x/*{bgActiveRepeat}*/;
	font-weight: normal/*{fwDefault}*/;
	color: #212121/*{fcActive}*/;
}
#ao3SearchForm .ui-state-active a,
#ao3SearchForm .ui-state-active a:link,
#ao3SearchForm .ui-state-active a:visited {
	color: #212121/*{fcActive}*/;
	text-decoration: none;
}

/* Interaction Cues
----------------------------------*/
#ao3SearchForm .ui-state-highlight,
#ao3SearchForm .ui-widget-content .ui-state-highlight,
#ao3SearchForm .ui-widget-header .ui-state-highlight {
	border: 1px solid #fcefa1/*{borderColorHighlight}*/;
	background: #fbf9ee/*{bgColorHighlight}*/ url("../assets/images/ui-bg_glass_55_fbf9ee_1x400.png")/*{bgImgUrlHighlight}*/ 50%/*{bgHighlightXPos}*/ 50%/*{bgHighlightYPos}*/ repeat-x/*{bgHighlightRepeat}*/;
	color: #363636/*{fcHighlight}*/;
}
#ao3SearchForm .ui-state-highlight a,
#ao3SearchForm .ui-widget-content .ui-state-highlight a,
#ao3SearchForm .ui-widget-header .ui-state-highlight a {
	color: #363636/*{fcHighlight}*/;
}
#ao3SearchForm .ui-state-error,
#ao3SearchForm .ui-widget-content .ui-state-error,
#ao3SearchForm .ui-widget-header .ui-state-error {
	border: 1px solid #cd0a0a/*{borderColorError}*/;
	background: #fef1ec/*{bgColorError}*/ url("../assets/images/ui-bg_glass_95_fef1ec_1x400.png")/*{bgImgUrlError}*/ 50%/*{bgErrorXPos}*/ 50%/*{bgErrorYPos}*/ repeat-x/*{bgErrorRepeat}*/;
	color: #cd0a0a/*{fcError}*/;
}
#ao3SearchForm .ui-state-error a,
#ao3SearchForm .ui-widget-content .ui-state-error a,
#ao3SearchForm .ui-widget-header .ui-state-error a {
	color: #cd0a0a/*{fcError}*/;
}
#ao3SearchForm .ui-state-error-text,
#ao3SearchForm .ui-widget-content .ui-state-error-text,
#ao3SearchForm .ui-widget-header .ui-state-error-text {
	color: #cd0a0a/*{fcError}*/;
}
#ao3SearchForm .ui-priority-primary,
#ao3SearchForm .ui-widget-content .ui-priority-primary,
#ao3SearchForm .ui-widget-header .ui-priority-primary {
	font-weight: bold;
}
#ao3SearchForm .ui-priority-secondary,
#ao3SearchForm .ui-widget-content .ui-priority-secondary,
#ao3SearchForm .ui-widget-header .ui-priority-secondary {
	opacity: .7;
	filter:Alpha(Opacity=70); /* support: IE8 */
	font-weight: normal;
}
#ao3SearchForm .ui-state-disabled,
#ao3SearchForm .ui-widget-content .ui-state-disabled,
#ao3SearchForm .ui-widget-header .ui-state-disabled {
	opacity: .35;
	filter:Alpha(Opacity=35); /* support: IE8 */
	background-image: none;
}
#ao3SearchForm .ui-state-disabled .ui-icon {
	filter:Alpha(Opacity=35); /* support: IE8 - See #6059 */
}

/* Icons
----------------------------------*/

/* states and images */
#ao3SearchForm .ui-icon {
	width: 16px;
	height: 16px;
}
#ao3SearchForm .ui-icon,
#ao3SearchForm .ui-widget-content .ui-icon {
	background-image: url("../assets/images/ui-icons_222222_256x240.png")/*{iconsContent}*/;
}
#ao3SearchForm .ui-widget-header .ui-icon {
	background-image: url("../assets/images/ui-icons_222222_256x240.png")/*{iconsHeader}*/;
}
#ao3SearchForm .ui-state-default .ui-icon {
	background-image: url("../assets/images/ui-icons_888888_256x240.png")/*{iconsDefault}*/;
}
#ao3SearchForm .ui-state-hover .ui-icon,
#ao3SearchForm .ui-state-focus .ui-icon {
	background-image: url("../assets/images/ui-icons_454545_256x240.png")/*{iconsHover}*/;
}
#ao3SearchForm .ui-state-active .ui-icon {
	background-image: url("../assets/images/ui-icons_454545_256x240.png")/*{iconsActive}*/;
}
#ao3SearchForm .ui-state-highlight .ui-icon {
	background-image: url("../assets/images/ui-icons_2e83ff_256x240.png")/*{iconsHighlight}*/;
}
#ao3SearchForm .ui-state-error .ui-icon,
#ao3SearchForm .ui-state-error-text .ui-icon {
	background-image: url("../assets/images/ui-icons_cd0a0a_256x240.png")/*{iconsError}*/;
}

/* positioning */
#ao3SearchForm .ui-icon-blank { background-position: 16px 16px; }
#ao3SearchForm .ui-icon-carat-1-n { background-position: 0 0; }
#ao3SearchForm .ui-icon-carat-1-ne { background-position: -16px 0; }
#ao3SearchForm .ui-icon-carat-1-e { background-position: -32px 0; }
#ao3SearchForm .ui-icon-carat-1-se { background-position: -48px 0; }
#ao3SearchForm .ui-icon-carat-1-s { background-position: -64px 0; }
#ao3SearchForm .ui-icon-carat-1-sw { background-position: -80px 0; }
#ao3SearchForm .ui-icon-carat-1-w { background-position: -96px 0; }
#ao3SearchForm .ui-icon-carat-1-nw { background-position: -112px 0; }
#ao3SearchForm .ui-icon-carat-2-n-s { background-position: -128px 0; }
#ao3SearchForm .ui-icon-carat-2-e-w { background-position: -144px 0; }
#ao3SearchForm .ui-icon-triangle-1-n { background-position: 0 -16px; }
#ao3SearchForm .ui-icon-triangle-1-ne { background-position: -16px -16px; }
#ao3SearchForm .ui-icon-triangle-1-e { background-position: -32px -16px; }
#ao3SearchForm .ui-icon-triangle-1-se { background-position: -48px -16px; }
#ao3SearchForm .ui-icon-triangle-1-s { background-position: -64px -16px; }
#ao3SearchForm .ui-icon-triangle-1-sw { background-position: -80px -16px; }
#ao3SearchForm .ui-icon-triangle-1-w { background-position: -96px -16px; }
#ao3SearchForm .ui-icon-triangle-1-nw { background-position: -112px -16px; }
#ao3SearchForm .ui-icon-triangle-2-n-s { background-position: -128px -16px; }
#ao3SearchForm .ui-icon-triangle-2-e-w { background-position: -144px -16px; }
#ao3SearchForm .ui-icon-arrow-1-n { background-position: 0 -32px; }
#ao3SearchForm .ui-icon-arrow-1-ne { background-position: -16px -32px; }
#ao3SearchForm .ui-icon-arrow-1-e { background-position: -32px -32px; }
#ao3SearchForm .ui-icon-arrow-1-se { background-position: -48px -32px; }
#ao3SearchForm .ui-icon-arrow-1-s { background-position: -64px -32px; }
#ao3SearchForm .ui-icon-arrow-1-sw { background-position: -80px -32px; }
#ao3SearchForm .ui-icon-arrow-1-w { background-position: -96px -32px; }
#ao3SearchForm .ui-icon-arrow-1-nw { background-position: -112px -32px; }
#ao3SearchForm .ui-icon-arrow-2-n-s { background-position: -128px -32px; }
#ao3SearchForm .ui-icon-arrow-2-ne-sw { background-position: -144px -32px; }
#ao3SearchForm .ui-icon-arrow-2-e-w { background-position: -160px -32px; }
#ao3SearchForm .ui-icon-arrow-2-se-nw { background-position: -176px -32px; }
#ao3SearchForm .ui-icon-arrowstop-1-n { background-position: -192px -32px; }
#ao3SearchForm .ui-icon-arrowstop-1-e { background-position: -208px -32px; }
#ao3SearchForm .ui-icon-arrowstop-1-s { background-position: -224px -32px; }
#ao3SearchForm .ui-icon-arrowstop-1-w { background-position: -240px -32px; }
#ao3SearchForm .ui-icon-arrowthick-1-n { background-position: 0 -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-ne { background-position: -16px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-e { background-position: -32px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-se { background-position: -48px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-s { background-position: -64px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-sw { background-position: -80px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-w { background-position: -96px -48px; }
#ao3SearchForm .ui-icon-arrowthick-1-nw { background-position: -112px -48px; }
#ao3SearchForm .ui-icon-arrowthick-2-n-s { background-position: -128px -48px; }
#ao3SearchForm .ui-icon-arrowthick-2-ne-sw { background-position: -144px -48px; }
#ao3SearchForm .ui-icon-arrowthick-2-e-w { background-position: -160px -48px; }
#ao3SearchForm .ui-icon-arrowthick-2-se-nw { background-position: -176px -48px; }
#ao3SearchForm .ui-icon-arrowthickstop-1-n { background-position: -192px -48px; }
#ao3SearchForm .ui-icon-arrowthickstop-1-e { background-position: -208px -48px; }
#ao3SearchForm .ui-icon-arrowthickstop-1-s { background-position: -224px -48px; }
#ao3SearchForm .ui-icon-arrowthickstop-1-w { background-position: -240px -48px; }
#ao3SearchForm .ui-icon-arrowreturnthick-1-w { background-position: 0 -64px; }
#ao3SearchForm .ui-icon-arrowreturnthick-1-n { background-position: -16px -64px; }
#ao3SearchForm .ui-icon-arrowreturnthick-1-e { background-position: -32px -64px; }
#ao3SearchForm .ui-icon-arrowreturnthick-1-s { background-position: -48px -64px; }
#ao3SearchForm .ui-icon-arrowreturn-1-w { background-position: -64px -64px; }
#ao3SearchForm .ui-icon-arrowreturn-1-n { background-position: -80px -64px; }
#ao3SearchForm .ui-icon-arrowreturn-1-e { background-position: -96px -64px; }
#ao3SearchForm .ui-icon-arrowreturn-1-s { background-position: -112px -64px; }
#ao3SearchForm .ui-icon-arrowrefresh-1-w { background-position: -128px -64px; }
#ao3SearchForm .ui-icon-arrowrefresh-1-n { background-position: -144px -64px; }
#ao3SearchForm .ui-icon-arrowrefresh-1-e { background-position: -160px -64px; }
#ao3SearchForm .ui-icon-arrowrefresh-1-s { background-position: -176px -64px; }
#ao3SearchForm .ui-icon-arrow-4 { background-position: 0 -80px; }
#ao3SearchForm .ui-icon-arrow-4-diag { background-position: -16px -80px; }
#ao3SearchForm .ui-icon-extlink { background-position: -32px -80px; }
#ao3SearchForm .ui-icon-newwin { background-position: -48px -80px; }
#ao3SearchForm .ui-icon-refresh { background-position: -64px -80px; }
#ao3SearchForm .ui-icon-shuffle { background-position: -80px -80px; }
#ao3SearchForm .ui-icon-transfer-e-w { background-position: -96px -80px; }
#ao3SearchForm .ui-icon-transferthick-e-w { background-position: -112px -80px; }
#ao3SearchForm .ui-icon-folder-collapsed { background-position: 0 -96px; }
#ao3SearchForm .ui-icon-folder-open { background-position: -16px -96px; }
#ao3SearchForm .ui-icon-document { background-position: -32px -96px; }
#ao3SearchForm .ui-icon-document-b { background-position: -48px -96px; }
#ao3SearchForm .ui-icon-note { background-position: -64px -96px; }
#ao3SearchForm .ui-icon-mail-closed { background-position: -80px -96px; }
#ao3SearchForm .ui-icon-mail-open { background-position: -96px -96px; }
#ao3SearchForm .ui-icon-suitcase { background-position: -112px -96px; }
#ao3SearchForm .ui-icon-comment { background-position: -128px -96px; }
#ao3SearchForm .ui-icon-person { background-position: -144px -96px; }
#ao3SearchForm .ui-icon-print { background-position: -160px -96px; }
#ao3SearchForm .ui-icon-trash { background-position: -176px -96px; }
#ao3SearchForm .ui-icon-locked { background-position: -192px -96px; }
#ao3SearchForm .ui-icon-unlocked { background-position: -208px -96px; }
#ao3SearchForm .ui-icon-bookmark { background-position: -224px -96px; }
#ao3SearchForm .ui-icon-tag { background-position: -240px -96px; }
#ao3SearchForm .ui-icon-home { background-position: 0 -112px; }
#ao3SearchForm .ui-icon-flag { background-position: -16px -112px; }
#ao3SearchForm .ui-icon-calendar { background-position: -32px -112px; }
#ao3SearchForm .ui-icon-cart { background-position: -48px -112px; }
#ao3SearchForm .ui-icon-pencil { background-position: -64px -112px; }
#ao3SearchForm .ui-icon-clock { background-position: -80px -112px; }
#ao3SearchForm .ui-icon-disk { background-position: -96px -112px; }
#ao3SearchForm .ui-icon-calculator { background-position: -112px -112px; }
#ao3SearchForm .ui-icon-zoomin { background-position: -128px -112px; }
#ao3SearchForm .ui-icon-zoomout { background-position: -144px -112px; }
#ao3SearchForm .ui-icon-search { background-position: -160px -112px; }
#ao3SearchForm .ui-icon-wrench { background-position: -176px -112px; }
#ao3SearchForm .ui-icon-gear { background-position: -192px -112px; }
#ao3SearchForm .ui-icon-heart { background-position: -208px -112px; }
#ao3SearchForm .ui-icon-star { background-position: -224px -112px; }
#ao3SearchForm .ui-icon-link { background-position: -240px -112px; }
#ao3SearchForm .ui-icon-cancel { background-position: 0 -128px; }
#ao3SearchForm .ui-icon-plus { background-position: -16px -128px; }
#ao3SearchForm .ui-icon-plusthick { background-position: -32px -128px; }
#ao3SearchForm .ui-icon-minus { background-position: -48px -128px; }
#ao3SearchForm .ui-icon-minusthick { background-position: -64px -128px; }
#ao3SearchForm .ui-icon-close { background-position: -80px -128px; }
#ao3SearchForm .ui-icon-closethick { background-position: -96px -128px; }
#ao3SearchForm .ui-icon-key { background-position: -112px -128px; }
#ao3SearchForm .ui-icon-lightbulb { background-position: -128px -128px; }
#ao3SearchForm .ui-icon-scissors { background-position: -144px -128px; }
#ao3SearchForm .ui-icon-clipboard { background-position: -160px -128px; }
#ao3SearchForm .ui-icon-copy { background-position: -176px -128px; }
#ao3SearchForm .ui-icon-contact { background-position: -192px -128px; }
#ao3SearchForm .ui-icon-image { background-position: -208px -128px; }
#ao3SearchForm .ui-icon-video { background-position: -224px -128px; }
#ao3SearchForm .ui-icon-script { background-position: -240px -128px; }
#ao3SearchForm .ui-icon-alert { background-position: 0 -144px; }
#ao3SearchForm .ui-icon-info { background-position: -16px -144px; }
#ao3SearchForm .ui-icon-notice { background-position: -32px -144px; }
#ao3SearchForm .ui-icon-help { background-position: -48px -144px; }
#ao3SearchForm .ui-icon-check { background-position: -64px -144px; }
#ao3SearchForm .ui-icon-bullet { background-position: -80px -144px; }
#ao3SearchForm .ui-icon-radio-on { background-position: -96px -144px; }
#ao3SearchForm .ui-icon-radio-off { background-position: -112px -144px; }
#ao3SearchForm .ui-icon-pin-w { background-position: -128px -144px; }
#ao3SearchForm .ui-icon-pin-s { background-position: -144px -144px; }
#ao3SearchForm .ui-icon-play { background-position: 0 -160px; }
#ao3SearchForm .ui-icon-pause { background-position: -16px -160px; }
#ao3SearchForm .ui-icon-seek-next { background-position: -32px -160px; }
#ao3SearchForm .ui-icon-seek-prev { background-position: -48px -160px; }
#ao3SearchForm .ui-icon-seek-end { background-position: -64px -160px; }
#ao3SearchForm .ui-icon-seek-start { background-position: -80px -160px; }
/* ui-icon-seek-first is deprecated, use ui-icon-seek-start instead */
#ao3SearchForm .ui-icon-seek-first { background-position: -80px -160px; }
#ao3SearchForm .ui-icon-stop { background-position: -96px -160px; }
#ao3SearchForm .ui-icon-eject { background-position: -112px -160px; }
#ao3SearchForm .ui-icon-volume-off { background-position: -128px -160px; }
#ao3SearchForm .ui-icon-volume-on { background-position: -144px -160px; }
#ao3SearchForm .ui-icon-power { background-position: 0 -176px; }
#ao3SearchForm .ui-icon-signal-diag { background-position: -16px -176px; }
#ao3SearchForm .ui-icon-signal { background-position: -32px -176px; }
#ao3SearchForm .ui-icon-battery-0 { background-position: -48px -176px; }
#ao3SearchForm .ui-icon-battery-1 { background-position: -64px -176px; }
#ao3SearchForm .ui-icon-battery-2 { background-position: -80px -176px; }
#ao3SearchForm .ui-icon-battery-3 { background-position: -96px -176px; }
#ao3SearchForm .ui-icon-circle-plus { background-position: 0 -192px; }
#ao3SearchForm .ui-icon-circle-minus { background-position: -16px -192px; }
#ao3SearchForm .ui-icon-circle-close { background-position: -32px -192px; }
#ao3SearchForm .ui-icon-circle-triangle-e { background-position: -48px -192px; }
#ao3SearchForm .ui-icon-circle-triangle-s { background-position: -64px -192px; }
#ao3SearchForm .ui-icon-circle-triangle-w { background-position: -80px -192px; }
#ao3SearchForm .ui-icon-circle-triangle-n { background-position: -96px -192px; }
#ao3SearchForm .ui-icon-circle-arrow-e { background-position: -112px -192px; }
#ao3SearchForm .ui-icon-circle-arrow-s { background-position: -128px -192px; }
#ao3SearchForm .ui-icon-circle-arrow-w { background-position: -144px -192px; }
#ao3SearchForm .ui-icon-circle-arrow-n { background-position: -160px -192px; }
#ao3SearchForm .ui-icon-circle-zoomin { background-position: -176px -192px; }
#ao3SearchForm .ui-icon-circle-zoomout { background-position: -192px -192px; }
#ao3SearchForm .ui-icon-circle-check { background-position: -208px -192px; }
#ao3SearchForm .ui-icon-circlesmall-plus { background-position: 0 -208px; }
#ao3SearchForm .ui-icon-circlesmall-minus { background-position: -16px -208px; }
#ao3SearchForm .ui-icon-circlesmall-close { background-position: -32px -208px; }
#ao3SearchForm .ui-icon-squaresmall-plus { background-position: -48px -208px; }
#ao3SearchForm .ui-icon-squaresmall-minus { background-position: -64px -208px; }
#ao3SearchForm .ui-icon-squaresmall-close { background-position: -80px -208px; }
#ao3SearchForm .ui-icon-grip-dotted-vertical { background-position: 0 -224px; }
#ao3SearchForm .ui-icon-grip-dotted-horizontal { background-position: -16px -224px; }
#ao3SearchForm .ui-icon-grip-solid-vertical { background-position: -32px -224px; }
#ao3SearchForm .ui-icon-grip-solid-horizontal { background-position: -48px -224px; }
#ao3SearchForm .ui-icon-gripsmall-diagonal-se { background-position: -64px -224px; }
#ao3SearchForm .ui-icon-grip-diagonal-se { background-position: -80px -224px; }


/* Misc visuals
----------------------------------*/

/* Corner radius */
#ao3SearchForm .ui-corner-all,
#ao3SearchForm .ui-corner-top,
#ao3SearchForm .ui-corner-left,
#ao3SearchForm .ui-corner-tl {
	border-top-left-radius: 4px/*{cornerRadius}*/;
}
#ao3SearchForm .ui-corner-all,
#ao3SearchForm .ui-corner-top,
#ao3SearchForm .ui-corner-right,
#ao3SearchForm .ui-corner-tr {
	border-top-right-radius: 4px/*{cornerRadius}*/;
}
#ao3SearchForm .ui-corner-all,
#ao3SearchForm .ui-corner-bottom,
#ao3SearchForm .ui-corner-left,
#ao3SearchForm .ui-corner-bl {
	border-bottom-left-radius: 4px/*{cornerRadius}*/;
}
#ao3SearchForm .ui-corner-all,
#ao3SearchForm .ui-corner-bottom,
#ao3SearchForm .ui-corner-right,
#ao3SearchForm .ui-corner-br {
	border-bottom-right-radius: 4px/*{cornerRadius}*/;
}

/* Overlays */
#ao3SearchForm .ui-widget-overlay {
	background: #aaaaaa/*{bgColorOverlay}*/ url("../assets/images/ui-bg_flat_0_aaaaaa_40x100.png")/*{bgImgUrlOverlay}*/ 50%/*{bgOverlayXPos}*/ 50%/*{bgOverlayYPos}*/ repeat-x/*{bgOverlayRepeat}*/;
	opacity: .3/*{opacityOverlay}*/;
	filter: Alpha(Opacity=30)/*{opacityFilterOverlay}*/; /* support: IE8 */
}
#ao3SearchForm .ui-widget-shadow {
	margin: -8px/*{offsetTopShadow}*/ 0 0 -8px/*{offsetLeftShadow}*/;
	padding: 8px/*{thicknessShadow}*/;
	background: #aaaaaa/*{bgColorShadow}*/ url("../assets/images/ui-bg_flat_0_aaaaaa_40x100.png")/*{bgImgUrlShadow}*/ 50%/*{bgShadowXPos}*/ 50%/*{bgShadowYPos}*/ repeat-x/*{bgShadowRepeat}*/;
	opacity: .3/*{opacityShadow}*/;
	filter: Alpha(Opacity=30)/*{opacityFilterShadow}*/; /* support: IE8 */
	border-radius: 8px/*{cornerRadiusShadow}*/;
}

/*!
 * jQuery UI Datepicker 1.8.23
 *
 * Copyright 2012, AUTHORS.txt (http://jqueryui.com/about)
 * Dual licensed under the MIT or GPL Version 2 licenses.
 * http://jquery.org/license
 *
 * http://docs.jquery.com/UI/Datepicker#theming
 */
.ui-datepicker { width: 17em; padding: .2em .2em 0; display: none; }
#ao3SearchForm .ui-datepicker { width: 17em; padding: .2em .2em 0; display: none; }
#ao3SearchForm .ui-datepicker .ui-datepicker-header { position:relative; padding:.2em 0; }
#ao3SearchForm .ui-datepicker .ui-datepicker-prev, .ui-datepicker .ui-datepicker-next { position:absolute; top: 2px; width: 1.8em; height: 1.8em; }
#ao3SearchForm .ui-datepicker .ui-datepicker-prev-hover, .ui-datepicker .ui-datepicker-next-hover { top: 1px; }
#ao3SearchForm .ui-datepicker .ui-datepicker-prev { left:2px; }
#ao3SearchForm .ui-datepicker .ui-datepicker-next { right:2px; }
#ao3SearchForm .ui-datepicker .ui-datepicker-prev-hover { left:1px; }
#ao3SearchForm .ui-datepicker .ui-datepicker-next-hover { right:1px; }
#ao3SearchForm .ui-datepicker .ui-datepicker-prev span, .ui-datepicker .ui-datepicker-next span { display: block; position: absolute; left: 50%; margin-left: -8px; top: 50%; margin-top: -8px;  }
#ao3SearchForm .ui-datepicker .ui-datepicker-title { margin: 0 2.3em; line-height: 1.8em; text-align: center; }
#ao3SearchForm .ui-datepicker .ui-datepicker-title select { font-size:1em; margin:1px 0; }
#ao3SearchForm .ui-datepicker select.ui-datepicker-month-year {width: 100%;}
#ao3SearchForm .ui-datepicker select.ui-datepicker-month, 
#ao3SearchForm .ui-datepicker select.ui-datepicker-year { width: 49%;}
#ao3SearchForm .ui-datepicker table {width: 100%; font-size: .9em; border-collapse: collapse; margin:0 0 .4em; }
#ao3SearchForm .ui-datepicker th { padding: .7em .3em; text-align: center; font-weight: bold; border: 0;  }
#ao3SearchForm .ui-datepicker td { border: 0; padding: 1px; }
#ao3SearchForm .ui-datepicker td span, .ui-datepicker td a { display: block; padding: .2em; text-align: right; text-decoration: none; }
#ao3SearchForm .ui-datepicker .ui-datepicker-buttonpane { background-image: none; margin: .7em 0 0 0; padding:0 .2em; border-left: 0; border-right: 0; border-bottom: 0; }
#ao3SearchForm .ui-datepicker .ui-datepicker-buttonpane button { float: right; margin: .5em .2em .4em; cursor: pointer; padding: .2em .6em .3em .6em; width:auto; overflow:visible; }
#ao3SearchForm .ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current { float:left; }

/* with multiple calendars */
#ao3SearchForm .ui-datepicker.ui-datepicker-multi { width:auto; }
#ao3SearchForm .ui-datepicker-multi .ui-datepicker-group { float:left; }
#ao3SearchForm .ui-datepicker-multi .ui-datepicker-group table { width:95%; margin:0 auto .4em; }
#ao3SearchForm .ui-datepicker-multi-2 .ui-datepicker-group { width:50%; }
#ao3SearchForm .ui-datepicker-multi-3 .ui-datepicker-group { width:33.3%; }
#ao3SearchForm .ui-datepicker-multi-4 .ui-datepicker-group { width:25%; }
#ao3SearchForm .ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header { border-left-width:0; }
#ao3SearchForm .ui-datepicker-multi .ui-datepicker-group-middle .ui-datepicker-header { border-left-width:0; }
#ao3SearchForm .ui-datepicker-multi .ui-datepicker-buttonpane { clear:left; }
#ao3SearchForm .ui-datepicker-row-break { clear:both; width:100%; font-size:0em; }

/* RTL support */
#ao3SearchForm .ui-datepicker-rtl { direction: rtl; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-prev { right: 2px; left: auto; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-next { left: 2px; right: auto; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-prev:hover { right: 1px; left: auto; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-next:hover { left: 1px; right: auto; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-buttonpane { clear:right; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-buttonpane button { float: left; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current { float:right; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-group { float:right; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header { border-right-width:0; border-left-width:1px; }
#ao3SearchForm .ui-datepicker-rtl .ui-datepicker-group-middle .ui-datepicker-header { border-right-width:0; border-left-width:1px; }

/* IE6 IFRAME FIX (taken from datepicker 1.5.3 */
#ao3SearchForm .ui-datepicker-cover {
    position: absolute; /*must have*/
    z-index: -1; /*must have*/
    filter: mask(); /*must have*/
    top: -4px; /*must have*/
    left: -4px; /*must have*/
    width: 200px; /*must have*/
    height: 200px; /*must have*/
}


/*!
 * jQuery UI Autocomplete 1.8.23
 *
 * Copyright 2012, AUTHORS.txt (http://jqueryui.com/about)
 * Dual licensed under the MIT or GPL Version 2 licenses.
 * http://jquery.org/license
 *
 * http://docs.jquery.com/UI/Autocomplete#theming
 */
#ao3SearchForm .ui-autocomplete { position: absolute; cursor: default; }	

/* workarounds */
* html #ao3SearchForm .ui-autocomplete { width:1px; } /* without this, the menu expands to 100% in IE6 */



/*
 * jQuery UI Menu 1.8.23
 *
 * Copyright 2010, AUTHORS.txt (http://jqueryui.com/about)
 * Dual licensed under the MIT or GPL Version 2 licenses.
 * http://jquery.org/license
 *
 * http://docs.jquery.com/UI/Menu#theming
 */
#ao3SearchForm .ui-menu {
	list-style:none;
	padding: 2px;
	margin: 0;
	display:block;
	float: left;
}
#ao3SearchForm .ui-menu .ui-menu {
	margin-top: -3px;
}
#ao3SearchForm .ui-menu .ui-menu-item {
	margin:0;
	padding: 0;
	zoom: 1;
	float: left;
	clear: left;
	width: 100%;
}
#ao3SearchForm .ui-menu .ui-menu-item a {
	text-decoration:none;
	display:block;
	padding:.2em .4em;
	line-height:1.5;
	zoom:1;
}
#ao3SearchForm .ui-menu .ui-menu-item a.ui-state-hover,
#ao3SearchForm .ui-menu .ui-menu-item a.ui-state-active {
	font-weight: normal;
	margin: -1px;
}


/*!
 * jQuery UI Selectmenu 1.11.4
 * http://jqueryui.com
 *
 * Copyright jQuery Foundation and other contributors
 * Released under the MIT license.
 * http://jquery.org/license
 *
 * http://api.jqueryui.com/selectmenu/#theming
 */
#ao3SearchForm .ui-selectmenu-menu {
	padding: 0;
	margin: 0;
	position: absolute;
	top: 0;
	left: 0;
	display: none;
}
#ao3SearchForm .ui-selectmenu-menu .ui-menu {
	overflow: auto;
	/* Support: IE7 */
	overflow-x: hidden;
	padding-bottom: 1px;
}
#ao3SearchForm .ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup {
	font-size: 1em;
	font-weight: bold;
	line-height: 1.5;
	padding: 2px 0.4em;
	margin: 0.5em 0 0 0;
	height: auto;
	border: 0;
}
#ao3SearchForm .ui-selectmenu-open {
	display: block;
}
#ao3SearchForm .ui-selectmenu-button {
	display: inline-block;
	overflow: hidden;
	position: relative;
	text-decoration: none;
	cursor: pointer;
}
#ao3SearchForm .ui-selectmenu-button span.ui-icon {
	right: 0.5em;
	left: auto;
	margin-top: -8px;
	position: absolute;
	top: 50%;
}
#ao3SearchForm .ui-selectmenu-button span.ui-selectmenu-text {
	text-align: left;
	padding: 0.4em 2.1em 0.4em 1em;
	display: block;
	line-height: 1.4;
	overflow: hidden;
	text-overflow: ellipsis;
	white-space: nowrap;
}

#ao3SearchForm .ui-autocomplete {
  font-size: 70%;
  text-align: left;
  max-height: 300px;
  max-width: 265px;
  overflow-y: auto;
  overflow-x: hidden;
}
#ao3SearchForm .ui-autocomplete li.odd a {
  background: #F5F5F5;
}
#ao3SearchForm .ui-autocomplete li.even a {
  background: white;
}
#ao3SearchForm .ui-autocomplete,
#ao3SearchForm .ui-autocomplete .ui-corner-all {
  border-radius: 0;
}
#ao3SearchForm .ui-autocomplete a {
  border: 1px solid white;
  font-weight: normal;
  overflow: hidden;
  color: #6E6E6E;
}
#ao3SearchForm .ui-autocomplete li a.ui-state-focus {
  color: white;
  background: #3399FF;
  font-weight: normal;
}
#ao3SearchForm .ui-autocomplete .child {
  padding-left: 25px;
  background: url('../assets/images/common/destchild.png') 15px center no-repeat;
}

#ao3SearchForm .ui-autocomplete .ui-menu-item {
  cursor: pointer;
}

#ao3SearchForm ul.ui-autocomplete.enableGoogleMapsLink li a .googleMapsLink {
  width: 10px;
  height: 20px;
  background: url('../assets/images/icon-googleMaps.png') no-repeat center center;
  position: absolute;
  top: 1px;
  right: 3px;
  cursor: pointer;
}

/* #ao3SearchForm ul.ui-autocomplete.enableGoogleMapsLink li a.ui-state-focus .googleMapsLink {
  background: url('../assets/images/icon-googleMaps-inverted.png') no-repeat center center;
} */

#ao3SearchForm ul.ui-autocomplete.enableGoogleMapsLink li {
  position: relative;
}

#ao3SearchForm ul.ui-autocomplete.enableGoogleMapsLink li a {
  padding-right: 15px;
}

html, html #ao3SearchForm .ui-widget {
  color: rgba(0, 0, 0, 0.87);
  font-family: "Roboto",sans-serif;
  font-weight: normal;
  line-height: 1.5;
}

html {
  font-size: 15px;
}

#ao3SearchForm select {
  font-size: 1.1em;
}

html #ao3SearchForm .ui-selectmenu-button span.ui-icon,
html #ao3SearchForm .ui-state-default .ui-icon-triangle-1-s,
html #ao3SearchForm .ui-icon-triangle-1-s {
  background: none;
  text-indent: 0;
  margin-top: -10px;
}

html #ao3SearchForm .ui-icon-triangle-1-s:before {
  font-family: 'gol-flights' !important;
  content: "V";
}

html #ao3SearchForm .ui-widget {
  font-size: 1em;
}

html #ao3SearchForm input.inputWithIconInside {
  padding-right: 2.1em;
  text-overflow: ellipsis;
  white-space: nowrap;
}

html #ao3SearchForm .ui-widget.ui-autocomplete {
  max-width: 100%;
}

html #ao3SearchForm body.transparentBody {
  background: transparent;
}

#ao3SearchForm .hidden {
  display: none;
}

#ao3SearchForm .ui-datepicker-current {
  display: none;
}

#ao3SearchForm input:not([type]), #ao3SearchForm input[type="text"], #ao3SearchForm input[type="password"], #ao3SearchForm input[type="email"], #ao3SearchForm input[type="url"], #ao3SearchForm input[type="time"], #ao3SearchForm input[type="date"], #ao3SearchForm input[type="datetime"], #ao3SearchForm input[type="datetime-local"], #ao3SearchForm input[type="tel"], #ao3SearchForm input[type="number"], #ao3SearchForm input[type="search"] {
  -moz-border-bottom-colors: none;
  -moz-border-left-colors: none;
  -moz-border-right-colors: none;
  -moz-border-top-colors: none;
  background-color: transparent;
  border-color: -moz-use-text-color -moz-use-text-color #9e9e9e;
  border-image: none;
  border-radius: 0;
  border-style: none none solid;
  border-width: medium medium 1px;
  box-shadow: none;
  box-sizing: border-box;
  font-size: 1rem;
  height: 3rem;
  margin: 0 0 15px;
  outline: medium none;
  padding: 0;
  transition: all 0.3s ease 0s;
  width: 100%;
}
#ao3SearchForm input:focus {
  border-bottom: 1px solid #26a69a;
  box-shadow: 0 1px 0 0 #26a69a;
}
#ao3SearchForm input::-ms-clear {
  display: none;
}
#ao3SearchForm input[type="submit"] {
  -moz-border-bottom-colors: none;
  -moz-border-left-colors: none;
  -moz-border-right-colors: none;
  -moz-border-top-colors: none;
  -webkit-appearance: none;
  border-color: -moz-use-text-color;
  border-image: none;
  border-radius: 0;
  border-style: none;
  border-width: medium;
  box-shadow: none;
  box-sizing: content-box;
  font-size: 1rem;
  height: 3rem;
  margin: 0;
  outline: medium none;
  padding: 0;
  transition: all 0.3s ease 0s;
  width: 100%;
}

#ao3SearchForm input.date {
  padding-left: 30px;
}

#ao3SearchForm .col.topGap {
  margin-top: 0.4rem;
}

#ao3SearchForm .iconInsideInput,
#ao3SearchForm .iconInsideInput2th,
#ao3SearchForm .iconInsideInputLeft {
  position: absolute;
  right: 1em;
  top: -1px;
  line-height: 3rem;
  height: 3rem;
}

#ao3SearchForm .iconInsideInputLeft {
  left: 1em;
  right: auto;
}

#ao3SearchForm .iconInsideInput2th {
  right: 2em;
}

#ao3SearchForm .j-flightSegmentHidden {
  display: none;
}

#ao3SearchForm .ui-selectmenu-button.ui-widget {
  border-radius: 0;
  background: inherit;
  border: none;
  border-color: -moz-use-text-color -moz-use-text-color #9e9e9e;
  border-image: none;
  border-style: none none solid;
  border-width: medium medium 1px;
  box-shadow: 0;
}

#ao3SearchForm .grey .ui-selectmenu-button.ui-widget {
  border-style: none;
}

#ao3SearchForm .ui-selectmenu-menu .ui-menu {
  padding: 0;
  max-height: 300px;
}
#ao3SearchForm .ui-selectmenu-menu .ui-menu-item {
  padding: 1px 2px;
  min-height: 1em;
}

#ao3SearchForm .ui-selectmenu-menu .ui-menu-item.ui-state-focus {
  background-image: none;
  border: none;

}

#ao3SearchForm .ui-autocomplete,
#ao3SearchForm .ui-selectmenu-open {
  box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
}

#ao3SearchForm .btn-icon {
    display: block;
    font-size: 32px;
    padding: 2px;
}

#ao3SearchForm .ui-button.ui-widget.ui-state-default,
#ao3SearchForm .activeBackground {
  background: #df5829;
  color: white;
}
#ao3SearchForm .tabActiveItem {
  color: white;
}

#ao3SearchForm .tabActiveItem .icon-oneway {
  background: #29b5f5;
}
#ao3SearchForm .tabActiveItem .icon-return {
  background: #df5829;
}
#ao3SearchForm .tabActiveItem .icon-multi {
  background: #b71b1b;
}

#ao3SearchForm .colorRemove {
  color: red;
}

#ao3SearchForm .colorError {
  color: red;
}

#ao3SearchForm .ui-dialog-buttonpane.ui-widget-content,
#ao3SearchForm .ui-dialog-content.ui-widget-content,
#ao3SearchForm .borderLess {
  border: none;
}

#ao3SearchForm .ui-dialog {
  box-shadow: 0 16px 28px 0 rgba(0, 0, 0, 0.22), 0 25px 55px 0 rgba(0, 0, 0, 0.21);
}
#ao3SearchForm .ui-dialog-buttonset {
  float: right;
}

#ao3SearchForm .ui-dialog-buttonset .ui-button {
  margin-right: 0.75rem;
  margin-bottom: 0.75rem;
  padding: 0.4em 1em;
  line-height: 1.4;
}

#ao3SearchForm .ui-dialog-titlebar {
  display: none;
}
#ao3SearchForm .cursorClickable {
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -khtml-user-select: none;
  -ms-user-select: none;
}

#ao3SearchForm .left {
  float: left;
}

#ao3SearchForm .right {
  float: right;
}

#ao3SearchForm.container {
  margin: 0 auto;
  max-width: 1280px;
  width: 90%;
  padding-bottom: 1rem;
  padding-top: 1rem;
}

@media only screen and (min-width: 601px) {
  #ao3SearchForm.container {
    width: 85%;
  }
}

#ao3SearchForm .white {
  background-color: #fff !important;
}

#ao3SearchForm .z-depth-1 {
  box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
}
#ao3SearchForm .grey.lighten-3 {
  background-color: #eee !important;
}
#ao3SearchForm .layer1 {
  position: relative;
  z-index: 100;
  background-color: rgb(102, 255, 0);
}
#ao3SearchForm .layer2 {
  margin: 0 10px;
}

#ao3SearchForm.container .row {
  margin-left: -0.75rem;
  margin-right: -0.75rem;
}

#ao3SearchForm .ui-dialog-content .row {
  margin-left: 0;
  margin-right: 0;
}

#ao3SearchForm .cleared,
.row:after {
  content: "";
  display: table;
  clear: both;
}

#ao3SearchForm .row .col {
  float: left;
  box-sizing: border-box;
  padding: 0 0.75rem;
}

#ao3SearchForm .col {
  margin: 0 auto;
  width: 83.3333%;
  position: relative;
}

#ao3SearchForm .row .col.s1 {
  width: 8.3333333333%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s2 {
  width: 16.6666666667%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s3 {
  width: 25%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s4 {
  width: 33.3333333333%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s5 {
  width: 41.6666666667%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s6 {
  width: 50%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s7 {
  width: 58.3333333333%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s8 {
  width: 66.6666666667%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s9 {
  width: 75%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s10 {
  width: 83.3333333333%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s11 {
  width: 91.6666666667%;
  margin-left: auto;
  left: auto;
  right: auto;
}

#ao3SearchForm .row .col.s12 {
  width: 100%;
  margin-left: auto;
  left: auto;
  right: auto;
}

@media only screen and (min-width: 993px) {
  #ao3SearchForm .row .col.l1 {
    width: 8.3333333333%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l2 {
    width: 16.6666666667%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l3 {
    width: 25%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l4 {
    width: 33.3333333333%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l5 {
    width: 41.6666666667%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l6 {
    width: 50%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l7 {
    width: 58.3333333333%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l8 {
    width: 66.6666666667%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l9 {
    width: 75%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l10 {
    width: 83.3333333333%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l11 {
    width: 91.6666666667%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
  #ao3SearchForm .row .col.l12 {
    width: 100%;
    margin-left: auto;
    left: auto;
    right: auto;
  }
}




</style>

